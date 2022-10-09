# Data Pipeline

Data Pipeline is a process whereby a data product pipeline deployment method is defined. Usually the deployment script contains the logic of the individual steps as well as the code chaining the steps together.

Data Pipeline enables building, deploying, and running the data product’s code, and storing and giving access to data and metadata. This priciple has been adopted from the [Data Mesh](https://towardsdatascience.com/what-is-a-data-mesh-and-how-not-to-mesh-it-up-210710bb41e0).

> Example of Data Pipeline component usage:

```javascript
  
"dataPipeline": {
  "infrastructure": {
    "platform": "Azure",
    "storageTechnology": "Azure SQL",
    "storageType": "sql",
    "containerTool": "helm",
    "format": "yaml",
    "status": "development",
    "scriptURL": "http://192.168.10.1/rundatapipeline.yml",
    "deploymentDocumentationURL": "http://192.168.10.1/datapipeline",
    "hashType": "SHA-2",
    "checksum": "7b7444ab8f5832e9ae8f54834782af995d0a83b4a1d77a75833eda7e19b4c921"
  }
  "dataAccess": {
    "outputPorttype": "API",
    "authenticationMethod": "OAuth",
    "specification": "OAS",
    "format": "GraphQL",
    "specURL": "https://192.168.10.1/petstore.json",
    "documentationURL": "http://192.168.10.1/petshop"
  }
}
  
```
| <div style="width:150px">Element name</div>   | Type  | Options  | Description  |
|---|---|---|---|
| infrastructure | element | - | Infrastructure is a process whereby a data product pipeline deployment method is defined. |
| platform | string | any | Platform infrastructure, such as AWS, GCP, Azure. |
| storageTechnology | string | any | Describes the internal storage area technology, such as Amazon S3, Google Cloud Storage, Azure Blob Storage, Azure SQL. |
| storageType | string | any | Describes the internal storage type, such as files, sql, events, MQTT. |
| containerTool | string | any | A name of the package manager, container or infrastructure as code tool. |
| format | string  | any |  Type of script language.|
| status | string  | Options: announcement, draft, development, testing, acceptance, production, sunset, retired. | Development status. |
| scriptURL | URL | Valid URL  | 	The URL of the deployment script. |
| deploymentDocumentationURL | URL | Valid URL  | 	The URL of the deployment documentation. |
| hashType| string | One of: SHA-1, SHA-2, SHA-3 | Type of secure hash algorithm for checksum. |
| checksum| string | any  | 	Script checksum. |
| dataAccess| element | - | Reference to the ability to use data. |
| outputPorttype | string | any  | 	Type of data access, such as API, SQL, sFTP, gRPC. |
| authenticationMethod | string | any  | Data access authentication method type, such as API key, HTTP Basic, OAuth, No authentication. |
| specification | string | any  | Type of the data access specification, such as OAS, RAML, Slate. |
| format | string | any | 	Data access file format type, such as JSON, XML, GraphQL, plain text. |
| specsURL | URL | Valid URL  | 	The URL of the specification. |
| documentationURL | URL | Valid URL  | The URL of the data access documentation. |

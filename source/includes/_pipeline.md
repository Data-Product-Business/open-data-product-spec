# Data Pipeline


Data Pipeline is a process whereby a data product pipeline deployment method is defined. Usually the deployment script contains the logic of the individual steps as well as the code chaining the steps together.

Data Pipeline Object's purpose is enabling building, deploying, and running the data product’s code, and storing and giving access to data and metadata. This priciple has been adopted from the [Data Mesh](https://towardsdatascience.com/what-is-a-data-mesh-and-how-not-to-mesh-it-up-210710bb41e0).

> Example of Data Pipeline component usage:

```javascript
  
"dataPipeline": {
  "infrastructure": {
    "containerTool": "helm",
    "format": "yaml",
    "status": "development",
    "scriptURL": "http://192.168.10.1/test/rundatapipeline.yml",
    "deploymentDocumentationURL": "http://192.168.10.1/test/docs/datapipeline",
    "hashType": "SHA-2",
    "checksum": "7b7444ab8f5832e9ae8f54834782af995d0a83b4a1d77a75833eda7e19b4c921"
  }, 
  "dataAccess" {
    "type": "API",
    "specification": "OAS",
    "format": "JSON",
    "specURL": "https://swagger.com/petstore.json",
    "dataAccessDocumentationURL": "http://192.168.10.1/test/docs/dataaccess"
  }
}

  
```
| <div style="width:150px">Element name</div>   | Type  | Options  | Description  |
|---|---|---|---|
| dataPipeline | element | - | Data Pipeline is a process whereby a data product pipeline deployment method is defined |
| containerTool | string | any | A name of the package manager, container or infrastructure as code tool |
| format | string  | any |  Type of script language|
| status | string  | Options: announcement, draft, development, testing, acceptance, production, sunset, retired |
| scriptURL | URL | Valid URL  | 	The URL of the deployment script. |
| deploymentDocumentationURL | URL | Valid URL  | 	The URL of the deployment documentation |
| hashType| string | One of: SHA-1, SHA-2, SHA-3 | Type of secure hash algorithm for checksum |
| checksum| string | any  | 	Script checksum |
| DataAccess | element | - | Reference to the ability to use data |
| type | string | One of: API, SQL, sFTP, gRPC  | 	Type of data access |
| specification | string | any  | Type of the data access specification |
| format | string | any  | 	File format |
| specsURL | URL | Valid URL  | 	The URL of the specification |
| dataAccessDocumentationURL | URL | Valid URL  | The URL of the data access documentation |


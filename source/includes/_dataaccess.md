# Data Access

Data access is the authorised ability to retrieve, edit, copy or transfer data from IT systems.

> Example of Data Access component usage:

```javascript
 
 "dataAccess": {
  "interface" {
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
| interface | element | - | Reference to the ability to use data. |
| outputPorttype | string | any  | 	Type of data access, such as API, SQL, sFTP, gRPC. |
| authenticationMethod | string | any  | Data access authentication method type, such as API key, HTTP Basic, OAuth, No authentication. |
| specification | string | any  | Type of the data access specification, such as OAS, RAML, Slate. |
| format | string | any | 	Data access file format type, such as JSON, XML, GraphQL, plain text. |
| specsURL | URL | Valid URL  | 	The URL of the specification. |
| documentationURL | URL | Valid URL  | The URL of the data access documentation. |

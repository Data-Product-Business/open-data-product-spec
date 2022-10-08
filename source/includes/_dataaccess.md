# Data Access

Data access is the authorised ability to retrieve, edit, copy or transfer data from IT systems.

> Example of Data Access component usage:

```javascript
 
 "dataAccess": {
  "interface" {
    "outputPorttype": "API",
    "authenticationMethod": "OAuth",
    "specification": "OAS",
    "format": "JSON",
    "specURL": "https://192.168.10.1/petstore.json",
    "documentationURL": "http://192.168.10.1/petshop"
  }
}
  
```
| <div style="width:150px">Element name</div>   | Type  | Options  | Description  |
|---|---|---|---|
| interface | element | - | Reference to the ability to use data. |
| outputPorttype | string | One of: API, SQL, sFTP, gRPC  | 	Type of data access. |
| authenticationMethod | string | One of: API key, HTTP Basic, OAuth, No authentication  | Data access authentication method type. |
| specification | string | any  | Type of the data access specification. |
| format | string | One of: JSON, XML, plain text | 	File format. |
| specsURL | URL | Valid URL  | 	The URL of the specification. |
| documentationURL | URL | Valid URL  | The URL of the data access documentation. |

# Data Access

Data access is the authorised ability to retrieve, edit, copy or transfer data from IT systems.

> Example of Data Access component usage:

```javascript
 
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
| dataAccess | element | - | Reference to the ability to use data. |
| type | string | One of: API, SQL, sFTP, gRPC  | 	Type of data access. |
| specification | string | any  | Type of the data access specification. |
| format | string | any  | 	File format. |
| specsURL | URL | Valid URL  | 	The URL of the specification. |
| dataAccessDocumentationURL | URL | Valid URL  | The URL of the data access documentation. |

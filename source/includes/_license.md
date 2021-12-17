# License

The data product may be exploited e.g. by licensing its use and exploitation to third parties. Machine-readable license as part of the specification is implemented for this purpose. It can be used to conclude various agreements regarding data protection, processing and intellectual property rights (IPR). Data can be protected by one or more intellectual property rights. Principle is that when a third party (Data User) exploits the data, it must have a license or other right from Data Holder to exploit to the data.

> Example of License Object usage:


```javascript
  
"license": {
   "scope": {
         "definition": "The purpose of this license is to determine the terms and conditions applicable to the licensing of the data product, whereby Data Holder grants Data User the right to use the data.",
         "language": "en-us",
         "permanent": false,
         "expiracyDate": "2022-12-15T00:00:00+02:00",
         "terminationContitions": "Cancellation before 30 days.",
         "continuityConditions": "Expired license will automatically continued without written cancellation (termination) by Data Holder",
         "restrictions": "Data User agrees not to, directly or indirectly, participate in the unauthorized use, disclosure or conversion of any confidential information.",      
         "geographicalArea": [ 
            "EU",
            "US"
         ],
         "modificationRight": true,
         "resellingRight": true,
         "roalties": "It is hereby agreed Data User shall share with Data Holder three percent (3%) of the revenues derives and receives from the usage their BI Dashbord solutions by the End Users.",
         "paymentsData User shall remit full payment within thirty (30) days after the end of each calendar month. Taxes (VAT 24 %) are included. Invoice will be electronical",
         "applicableLaws": "This license shall be interpreted, construed and enforced in accordance with the law of Finland. Copyright: 2021 Mindmote Oy"
            }
   "governance": {
         "containsPersonalData": true,
         "dpaURL": "http://192.168.10.1/dpaconditions",
         "audit": "Audit is conducted in accordance with the Petshop´s Data-audits ltd., www.petshopsdataaudits.com",
         "warranties": "The Data User agrees that the following disclaimers apply to its customers and/or other entities.",
         "forceMajeure": "Each party may suspend the fulfilment of its contractual obligations, when the said fulfilment is impossible or objectively too costly due to an unforeseeable impediment independent from the parties, such as for example: strike, boycott, lockout, fire, war (declared or not), civil war, riots and revolutions, requisitions, embargo, power blackouts, extraordinary breakage of machinery, delays in the delivery of components or raw materials.",
         "damages": "During the term of license, except for the force majeure or the Data Holders reasons, Data User is required to follow strictly in accordance with the license. If Data User wants to terminate the license early, it needs to pay a certain amount of liquidated damages.",
         "confidentiality": "Data User undertakes to maintain confidentiality as regards all information of a technical (such as, by way of a non-limiting example, drawings, tables, documentation, formulas and correspondence) and commercial nature (including contractual conditions, prices, payment conditions) gained during the performance of this license."          
   }
  }
}

  
```
| <div style="width:150px">Element name</div>   | Type  | Options  | Description  |
|---|---|---|---|
| definition | string | text content, max length 512 chars  | Background and purpose of the license |
| language | string | ISO 639-1 standard language codes | License language |
| permanent | boolean | true/false|  License with no expiration date |
| expiracyDate | DateTime | A combination of date and time in ISO 8601 format yyyy-MM-dd'T'HH:mm:ss.SSSZ. | License expiration date |
| termitationContitions | string | text content, max length 512 chars | Cancellation of the license |
| continuityConditions | string |  text content, max length 512 chars | Continuity of the license |
| restrictions | string | text content, max length 512 chars  | Restrictions of the license |
| geographicalArea | string |  ISO 3166-1 alpha-2 codes | License right shall be restricted to the geographical area |
| modificationRights | boolean | true/false | Data modification rights |
| resellingRights | boolean | true/false | Reselling rights |
| royalties | string | text content, max length 512 chars | License royalties |
| applicableLaws | string | text content, max length 512 chars | Applicable laws i.e intellectual property right |
| containsPersonalData | boolean | true/false | Data contains personal data |
| dpaURL| URL| Valid URL | The URL of the data processing agreement |
| audit | string | text content, max length 512 chars | License auditing |
| warranties | string | text content, max length 512 chars | License warranties |
| forceMajeure | string | text content, max length 512 chars | Force Majeure |
| damages| string | text content, max length 512 chars | Damages refers to the sum of money (i.e. indemnifications) for a breach of some duty or violation of license right. |
| confidentiality | string | text content, max length 512 chars| Restrictions and requirements imposed on the Data User regarding e.g. the use and disclosure of the Data Holder's confidential information. |
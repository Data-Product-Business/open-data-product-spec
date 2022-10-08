# Hello world example

You'll find a complete machine-readbale example of a data product from the right column. It is imaginary data product *Pets of the year* which contains derived data about the most common pets in the world. The product has 4 pricing plans which are mostly based on recurring subscription model. Note! Not all voluntary attributes are used in the example.  

> Example of complete working Data Product specification instance:

```javascript
{
	"Product": {
		"name": "Pets of the year",
		"productID": "123456are",
		"description": "",
		"visibility": "private",
		"status": "draft",
		"version": "0.1",
		"categories": ["pets"],
		"tags": ["pet"],
		"brandSlogan": "Passion for the data monetization",
		"type": "derived data",
		"logoURL": "https://data-product-business.github.io/open-data-product-spec/images/logo-dps-ebd5a97d.png"
	},
	"pricing": [{
			"name": "Premium subscription 1 year",
			"priceCurrency": "EUR",
			"price": "50.00",
			"billingDuration": "year",
			"unit": "recurring",
			"maxTransactionQuantity": "unlimited"
		},
		{
			"name": "Premium Package Monthly",
			"priceCurrency": "EUR",
			"price": "5.00",
			"billingDuration": "month",
			"unit": "recurring",
			"maxTransactionQuantity": 10000
		},
		{
			"name": "Freemium Package",
			"priceCurrency": "EUR",
			"price": "0.00",
			"billingDuration": "month",
			"unit": "recurring",
			"maxTransactionQuantity": 1000
		},
		{
			"name": "Revenue sharing",
			"priceCurrency": "percentage",
			"price": "5.50",
			"billingDuration": "month",
			"unit": "revenue-sharing",
			"maxTransactionQuantity": 20000
		}
	],

	"dataOps": {
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
	},
	"dataAccess": {
		"type": "API",
    "authenticationMethod": "OAuth",
		"specification": "OAS",
		"format": "JSON",
		"specURL": "https://swagger.com/petstore.json",
		"dataAccessDocumentationURL": "http://192.168.10.1/test/docs/dataaccess"
	},
	"SLA": {
		"updateFrequency": {
			"unit": "hours",
			"value": 1
		},
		"uptime": {
			"unit": "percentage",
			"value": 99
		},
		"responseTime": {
			"unit": "milliseconds",
			"value": 200
		},
		"nullValues": {
			"unit": "percentage",
			"value": 0.01
		},
		"support": {
			"company": {
				"phoneNumber": "",
				"phoneServiceHours": "",
				"chatURL": "",
				"chatServiceHours": "",
				"chatResponseTime": "",
				"email": "",
				"emailServiceHours": "",
				"emailResponseTime": "",
				"documentationURL": "",
				"guidesURL": ""
			},
			"community": {
				"stackoverflowURL": "",
				"forumURL": "",
				"slackURL": "",
				"twitterURL": ""
			}
		},
		"observability": {
			"logsURL": "https://logs.com",
			"dashboardURL": "https://dashboard.com",
			"uptimeURL": "https://uptime.com"
		}
	},
	"license": {
		"scope": {
			"definition": "The purpose of this license is to determine the terms and conditions applicable to the licensing of the data product, whereby Data Holder grants Data User the right to use the data.",
			"language": "en-us",
			"permanent": false,
			"terminationContitions": "Cancellation before 30 days. After the expiry of the right of use, the product and its derivatives must be removed.",
			"continuityConditions": "Expired license will automatically continued without written cancellation (termination) by Data Holder",
			"restrictions": "Data User agrees not to, directly or indirectly, participate in the unauthorized use, disclosure or conversion of any confidential information.",
			"geographicalArea": [
				"EU",
				"US"
			],
			"modificationRight": true,
			"resellingRight": true
		},
		"governance": {
			"containsPersonalData": true,
			"dpaURL": "http://192.168.10.1/dpaconditions",
			"audit": "Data Holder will reasonably cooperate with Data User by providing available additional information concerning the data product. Each party will bear its own costs with respect to the audit procedures.",
			"warranties": "Data Holder makes no warranties, express or implied, guarantees or conditions with respect to your use of the data product. To the extent permitted under local law, Data Holder disclaims all liability for any damages or losses, including direct, consequential, special, indirect, incidental or punitive, resulting from Data User use of the data product.",
			"forceMajeure": "Each party may suspend the fulfilment of its contractual obligations, when the said fulfilment is impossible or objectively too costly due to an unforeseeable impediment independent from the parties, such as for example: strike, boycott, lockout, fire, war (declared or not), civil war, riots and revolutions, requisitions, embargo, power blackouts, extraordinary breakage of machinery, delays in the delivery of components or raw materials.",
			"damages": "During the term of license, except for the force majeure or the Data Holders reasons, Data User is required to follow strictly in accordance with the license. If Data User wants to terminate the license early, it needs to pay a certain amount of liquidated damages.",
			"confidentiality": "Data User undertakes to maintain confidentiality as regards all information of a technical (such as, by way of a non-limiting example, drawings, tables, documentation, formulas and correspondence) and commercial nature (including contractual conditions, prices, payment conditions) gained during the performance of this license.",
			"applicableLaws": "This license shall be interpreted, construed and enforced in accordance with the law of Finland, Incl. Copyright Act 404/1961."
		}
	},
	"dataHolder": {
		"taxID": "12243434-12",
		"vatID": "12243434-12",
		"logoURL": "https://mindmote.fi/logo.png",
		"description": "Digital Economy services and tools",
		"URL": "https://mindmote.fi",
		"telephone": "+35845 0232 2323",
		"streetAddress": "Koulukatu 1",
		"postalCode": "33100",
		"addressRegion": "Pirkanmaa",
		"addressLocality": "Tampere",
		"addressCountry": "Finland",
		"aggregateRating": "",
		"ratingCount": 1245,
		"slogan": "",
		"parentOrganization": ""
	}
}
```

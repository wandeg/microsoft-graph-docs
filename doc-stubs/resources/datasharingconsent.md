---
title: "dataSharingConsent resource type"
description: "Data sharing consent information."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# dataSharingConsent resource type


Namespace: microsoft.graph

Data sharing consent information.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[consentToDataSharing](../api/datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/datasharingconsent.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|grantDateTime|DateTimeOffset|The time consent was granted for this account|
|granted|Boolean|The granted state for the data sharing consent|
|grantedByUpn|String|The Upn of the user that granted consent for this account|
|grantedByUserId|String|The UserId of the user that granted consent for this account|
|id|String|The data sharing consent Id|
|serviceDisplayName|String|The display name of the service work flow|
|termsUrl|String|The TermsUrl for the data sharing consent|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.dataSharingConsent",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": "Boolean",
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```


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


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get dataSharingConsent](../api/datasharingconsent-get.md)|[dataSharingConsent](../resources/datasharingconsent.md)|Read the properties and relationships of a [dataSharingConsent](../resources/datasharingconsent.md) object.|
|[Update dataSharingConsent](../api/datasharingconsent-update.md)|[dataSharingConsent](../resources/datasharingconsent.md)|Update the properties of a [dataSharingConsent](../resources/datasharingconsent.md) object.|
|[consentToDataSharing](../api/datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/datasharingconsent.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|grantDateTime|DateTimeOffset|The time consent was granted for this account|
|granted|Boolean|The granted state for the data sharing consent|
|grantedByUpn|String|The Upn of the user that granted consent for this account|
|grantedByUserId|String|The UserId of the user that granted consent for this account|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|serviceDisplayName|String|The display name of the service work flow|
|termsUrl|String|The TermsUrl for the data sharing consent|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```


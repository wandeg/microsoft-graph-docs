---
title: "companyInformation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# companyInformation resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postaladdresstype.md)|**TODO: Add Description**|
|currencyCode|String|**TODO: Add Description**|
|currentFiscalYearStartDate|Date|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|email|String|**TODO: Add Description**|
|faxNumber|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|industry|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|phoneNumber|String|**TODO: Add Description**|
|picture|Stream|**TODO: Add Description**|
|taxRegistrationNumber|String|**TODO: Add Description**|
|website|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.companyInformation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.companyInformation",
  "id": "String (identifier)",
  "displayName": "String",
  "address": {
    "@odata.type": "microsoft.graph.postalAddressType"
  },
  "phoneNumber": "String",
  "faxNumber": "String",
  "email": "String",
  "website": "String",
  "taxRegistrationNumber": "String",
  "currencyCode": "String",
  "currentFiscalYearStartDate": "Date",
  "industry": "String",
  "picture": "Stream",
  "lastModifiedDateTime": "String (timestamp)"
}
```


---
title: "companyInformation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# companyInformation resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get companyInformation](../api/companyinformation-get.md)|[companyInformation](../resources/companyinformation.md)|Read properties and relationships of the [companyInformation](../resources/companyinformation.md) object.|
|[Update companyInformation](../api/companyinformation-update.md)|[companyInformation](../resources/companyinformation.md)|Update the properties of a [companyInformation](../resources/companyinformation.md) object.|
|[List companyInformation](../api/company-list-companyinformation.md)|[companyInformation](../resources/companyinformation.md) collection|Get the companyInformations from the companyInformation navigation property.|
|[Add companyInformation](../api/company-post-companyinformation.md)|[companyInformation](../resources/companyinformation.md)|Add companyInformation by posting to the companyInformation collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[postalAddressType](../resources/postaladdresstype.md)||
|currencyCode|String||
|currentFiscalYearStartDate|Date||
|displayName|String||
|email|String||
|faxNumber|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|industry|String||
|lastModifiedDateTime|DateTimeOffset||
|phoneNumber|String||
|picture|Stream||
|taxRegistrationNumber|String||
|website|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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


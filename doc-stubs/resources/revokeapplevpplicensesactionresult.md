---
title: "revokeAppleVppLicensesActionResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# revokeAppleVppLicensesActionResult resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [deviceActionResult](../resources/deviceactionresult.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionName|String|**TODO: Add Description** Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|actionState|actionState|**TODO: Add Description** Inherited from [deviceActionResult](../resources/deviceactionresult.md). Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|failedLicensesCount|Int32|**TODO: Add Description**|
|lastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|startDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [deviceActionResult](../resources/deviceactionresult.md)|
|totalLicensesCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.revokeAppleVppLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.revokeAppleVppLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": "Integer",
  "failedLicensesCount": "Integer"
}
```


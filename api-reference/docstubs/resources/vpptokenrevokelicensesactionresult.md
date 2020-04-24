---
title: "vppTokenRevokeLicensesActionResult resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# vppTokenRevokeLicensesActionResult resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [vppTokenActionResult](../resources/vpptokenactionresult.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionFailureReason|vppTokenActionFailureReason|The reason for the revoke licenses action failure. Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
|actionName|String|Action name Inherited from [vppTokenActionResult](../resources/vpptokenactionresult.md)|
|actionState|actionState|State of the action Inherited from [vppTokenActionResult](../resources/vpptokenactionresult.md). Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|failedLicensesCount|Int32|A count of the number of licenses that failed to revoke.|
|lastUpdatedDateTime|DateTimeOffset|Time the action state was last updated Inherited from [vppTokenActionResult](../resources/vpptokenactionresult.md)|
|startDateTime|DateTimeOffset|Time the action was initiated Inherited from [vppTokenActionResult](../resources/vpptokenactionresult.md)|
|totalLicensesCount|Int32|A count of the number of licenses that were attempted to revoke.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenRevokeLicensesActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenRevokeLicensesActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "totalLicensesCount": 1024,
  "failedLicensesCount": 1024,
  "actionFailureReason": "String"
}
```


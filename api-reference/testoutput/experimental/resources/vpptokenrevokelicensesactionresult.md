---
title: "vppTokenRevokeLicensesActionResult resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# vppTokenRevokeLicensesActionResult resource type




Inherits from [vppTokenActionResult](../resources/vppTokenActionResult.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|actionFailureReason|Enumeration|The reason for the revoke licenses action failure. Possible values are: `none`, `appleFailure`, `internalError`, `expiredVppToken`, `expiredApplePushNotificationCertificate`.|
|actionName|String|Action name Inherited from [vppTokenActionResult](../resources/vppTokenActionResult.md)|
|actionState|Enumeration|State of the action Inherited from [vppTokenActionResult](../resources/vppTokenActionResult.md). Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|failedLicensesCount|Int32|A count of the number of licenses that failed to revoke.|
|lastUpdatedDateTime|DateTimeOffset|Time the action state was last updated Inherited from [vppTokenActionResult](../resources/vppTokenActionResult.md)|
|startDateTime|DateTimeOffset|Time the action was initiated Inherited from [vppTokenActionResult](../resources/vppTokenActionResult.md)|
|totalLicensesCount|Int32|A count of the number of licenses that were attempted to revoke.|

## Relationships
None

## JSON Representation
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


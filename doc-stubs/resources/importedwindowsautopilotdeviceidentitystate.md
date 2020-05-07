---
title: "importedWindowsAutopilotDeviceIdentityState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# importedWindowsAutopilotDeviceIdentityState resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceErrorCode|Int32|**TODO: Add Description**|
|deviceErrorName|String|**TODO: Add Description**|
|deviceImportStatus|importedWindowsAutopilotDeviceIdentityImportStatus|**TODO: Add Description**. Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.|
|deviceRegistrationId|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
  "deviceImportStatus": "String",
  "deviceRegistrationId": "String",
  "deviceErrorCode": "Integer",
  "deviceErrorName": "String"
}
```


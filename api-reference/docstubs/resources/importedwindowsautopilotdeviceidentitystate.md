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
|deviceErrorCode|Int32|Device error code reported by Device Directory Service(DDS).|
|deviceErrorName|String|Device error name reported by Device Directory Service(DDS).|
|deviceImportStatus|importedWindowsAutopilotDeviceIdentityImportStatus|Device status reported by Device Directory Service(DDS). Possible values are: `unknown`, `pending`, `partial`, `complete`, `error`.|
|deviceRegistrationId|String|Device Registration ID for successfully added device reported by Device Directory Service(DDS).|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "deviceErrorCode": 1024,
  "deviceErrorName": "String"
}
```


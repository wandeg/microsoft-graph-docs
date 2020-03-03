---
title: "importedWindowsAutopilotDeviceIdentityUpload resource type"
description: "Import windows autopilot devices using upload."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# importedWindowsAutopilotDeviceIdentityUpload resource type


Namespace: microsoft.graph

Import windows autopilot devices using upload.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List importedWindowsAutopilotDeviceIdentityUploads](../api/importedwindowsautopilotdeviceidentityupload-list.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) collection|List properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) objects.|
|[Get importedWindowsAutopilotDeviceIdentityUpload](../api/importedwindowsautopilotdeviceidentityupload-get.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md)|Read properties and relationships of the [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) object.|
|[Create importedWindowsAutopilotDeviceIdentityUpload](../api/importedwindowsautopilotdeviceidentityupload-create.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md)|Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) object.|
|[Delete importedWindowsAutopilotDeviceIdentityUpload](../api/importedwindowsautopilotdeviceidentityupload-delete.md)|None|Deletes a [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md).|
|[Update importedWindowsAutopilotDeviceIdentityUpload](../api/importedwindowsautopilotdeviceidentityupload-update.md)|[importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md)|Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/importedwindowsautopilotdeviceidentityupload.md) object.|
|[List deviceIdentities](../api/importedwindowsautopilotdeviceidentityupload-list-deviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|Get the importedWindowsAutopilotDeviceIdentities from the deviceIdentities navigation property.|
|[Add deviceIdentities](../api/importedwindowsautopilotdeviceidentityupload-post-deviceidentities.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md)|Add deviceIdentities by posting to the deviceIdentities collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTimeUtc|DateTimeOffset|DateTime when the entity is created.|
|id|String| Inherited from [entity](../resources/entity.md)|
|status|Enumeration|Upload status. Possible values are: `noUpload`, `pending`, `complete`, `error`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|deviceIdentities|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|Collection of all Autopilot devices as a part of this upload.|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "String (identifier)",
  "createdDateTimeUtc": "String (timestamp)",
  "status": "String"
}
```


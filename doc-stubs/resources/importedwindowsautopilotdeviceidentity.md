---
title: "importedWindowsAutopilotDeviceIdentity resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# importedWindowsAutopilotDeviceIdentity resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[import](../api/importedwindowsautopilotdeviceidentity-import.md)|[importedWindowsAutopilotDeviceIdentity](../resources/importedwindowsautopilotdeviceidentity.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|assignedUserPrincipalName|String|**TODO: Add Description**|
|groupTag|String|**TODO: Add Description**|
|hardwareIdentifier|Binary|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|importId|String|**TODO: Add Description**|
|orderIdentifier|String|**TODO: Add Description**|
|productKey|String|**TODO: Add Description**|
|serialNumber|String|**TODO: Add Description**|
|state|[importedWindowsAutopilotDeviceIdentityState](../resources/importedwindowsautopilotdeviceidentitystate.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
  "id": "String (identifier)",
  "orderIdentifier": "String",
  "groupTag": "String",
  "serialNumber": "String",
  "productKey": "String",
  "importId": "String",
  "hardwareIdentifier": "Binary",
  "state": {
    "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState"
  },
  "assignedUserPrincipalName": "String"
}
```


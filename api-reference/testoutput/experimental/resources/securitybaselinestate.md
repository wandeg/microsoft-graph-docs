---
title: "securityBaselineState resource type"
description: "Security baseline state for a device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# securityBaselineState resource type


Namespace: microsoft.graph

Security baseline state for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityBaselineState](../api/securitybaselinestate-get.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Read properties and relationships of the [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[Update securityBaselineState](../api/securitybaselinestate-update.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Update the properties of a [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[List settingStates](../api/securitybaselinestate-list-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md) collection|Get the securityBaselineSettingStates from the settingStates navigation property.|
|[Add settingStates](../api/securitybaselinestate-post-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Add settingStates by posting to the settingStates collection.|
|[List securityBaselineStates](../api/manageddevice-list-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md) collection|Get the securityBaselineStates from the securityBaselineStates navigation property.|
|[Add securityBaselineStates](../api/manageddevice-post-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Add securityBaselineStates by posting to the securityBaselineStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name of the security baseline|
|id|String| Inherited from [entity](../resources/entity.md)|
|securityBaselineTemplateId|String|The security baseline template id|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|settingStates|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md) collection|The security baseline state for different settings for a device|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineState",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "String (identifier)",
  "securityBaselineTemplateId": "String",
  "displayName": "String"
}
```


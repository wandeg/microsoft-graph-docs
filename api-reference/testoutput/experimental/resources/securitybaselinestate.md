---
title: "securityBaselineState resource type"
description: "Security baseline state for a device."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# securityBaselineState resource type

Security baseline state for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityBaselineState](../api/securitybaselinestate-get.md)|[securityBaselineState](../resources/securityBaselineState.md)|Read properties and relationships of the [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[Delete securityBaselineState](../api/securitybaselinestate-delete.md)|None|Deletes a [securityBaselineState](../resources/securitybaselinestate.md).|
|[Update securityBaselineState](../api/securitybaselinestate-update.md)|[securityBaselineState](../resources/securityBaselineState.md)|Update the properties of a [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[List settingStates](../api/securitybaselinestate-list-settingstates.md)|[securityBaselineSettingState](../resources/securityBaselineSettingState.md) collection|Get the securityBaselineSettingStates from the settingStates navigation property.|
|[Add settingStates](../api/securitybaselinestate-post-settingstates.md)|[securityBaselineSettingState](../resources/securityBaselineSettingState.md)|Add settingStates by posting to the settingStates collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name of the security baseline|
|id|String| Inherited from [entity](../resources/entity.md)|
|securityBaselineTemplateId|String|The security baseline template id|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|settingStates|[securityBaselineSettingState](../resources/securityBaselineSettingState.md) collection|The security baseline state for different settings for a device|

## JSON Representation
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


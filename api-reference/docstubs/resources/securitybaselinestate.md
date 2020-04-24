---
title: "securityBaselineState resource type"
description: "Security baseline state for a device."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# securityBaselineState resource type


Namespace: microsoft.graph

Security baseline state for a device.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get securityBaselineState](../api/securitybaselinestate-get.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Read the properties and relationships of a [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[Update securityBaselineState](../api/securitybaselinestate-update.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Update the properties of a [securityBaselineState](../resources/securitybaselinestate.md) object.|
|[List settingStates](../api/securitybaselinestate-list-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md) collection|Get the securityBaselineSettingStates from the settingStates navigation property.|
|[Create settingStates](../api/securitybaselinestate-post-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Create a new settingStates object.|
|[Delete settingStates](../api/securitybaselinestate-delete-settingstates.md)|None|Delete a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|
|[Update settingStates](../api/securitybaselinestate-update-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Update the properties of a settingStates object.|
|[Get securityBaselineSettingState](../api/securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Read the properties and relationships of a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The display name of the security baseline|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
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


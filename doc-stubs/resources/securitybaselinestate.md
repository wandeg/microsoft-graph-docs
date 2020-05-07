---
title: "securityBaselineState resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# securityBaselineState resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List settingStates](../api/securitybaselinestate-list-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md) collection|Get the securityBaselineSettingStates from the settingStates navigation property.|
|[Create settingStates](../api/securitybaselinestate-post-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Create a new settingStates object.|
|[Delete settingStates](../api/securitybaselinestate-delete-settingstates.md)|None|Delete a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|
|[Update settingStates](../api/securitybaselinestate-update-settingstates.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Update the properties of a settingStates object.|
|[Get securityBaselineSettingState](../api/securitybaselinesettingstate-get.md)|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md)|Read the properties and relationships of a [securityBaselineSettingState](../resources/securitybaselinesettingstate.md) object.|
|[List securityBaselineStates](../api/manageddevice-list-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md) collection|Get the securityBaselineStates from the securityBaselineStates navigation property.|
|[Create securityBaselineStates](../api/manageddevice-post-securitybaselinestates.md)|[securityBaselineState](../resources/securitybaselinestate.md)|Create a new securityBaselineStates object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|securityBaselineTemplateId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|settingStates|[securityBaselineSettingState](../resources/securitybaselinesettingstate.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
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


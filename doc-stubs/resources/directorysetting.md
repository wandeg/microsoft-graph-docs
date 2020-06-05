---
title: "directorySetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# directorySetting resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List settings](../api/group-list-settings.md)|[directorySetting](../resources/directorysetting.md) collection|Get the directorySettings from the settings navigation property.|
|[Create settings](../api/group-post-settings.md)|[directorySetting](../resources/directorysetting.md)|Create a new settings object.|
|[Update settings](../api/group-update-settings.md)|[directorySetting](../resources/directorysetting.md)|Update the properties of a settings object.|
|[Get settings](../api/group-get-directorysetting.md)|[directorySetting](../resources/directorysetting.md)|Read the properties and relationships of a [directorySetting](../resources/directorysetting.md) object.|
|[Delete settings](../api/group-delete-settings.md)|None|Delete a [directorySetting](../resources/directorysetting.md) object.|
|[List directorySettings](../api/directorysetting-list.md)|[directorySetting](../resources/directorysetting.md) collection|Get a list of the [directorySetting](../resources/directorysetting.md) objects and their properties.|
|[Create directorySetting](../api/directorysetting-post-settings.md)|[directorySetting](../resources/directorysetting.md)|Create a new [directorySetting](../resources/directorysetting.md) object.|
|[Get directorySetting](../api/directorysetting-get.md)|[directorySetting](../resources/directorysetting.md)|Read the properties and relationships of a [directorySetting](../resources/directorysetting.md) object.|
|[Update directorySetting](../api/directorysetting-update.md)|[directorySetting](../resources/directorysetting.md)|Update the properties of a [directorySetting](../resources/directorysetting.md) object.|
|[Delete directorySetting](../api/directorysetting-delete.md)|None|Deletes a [directorySetting](../resources/directorysetting.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|templateId|String|**TODO: Add Description**|
|values|[settingValue](../resources/settingvalue.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directorySetting",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directorySetting",
  "id": "String (identifier)",
  "displayName": "String",
  "templateId": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingValue"
    }
  ]
}
```


---
title: "directorySetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# directorySetting resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get directorySetting](../api/directorysetting-get.md)|[directorySetting](../resources/directorySetting.md)|Read properties and relationships of the [directorySetting](../resources/directorysetting.md) object.|
|[Delete directorySetting](../api/directorysetting-delete.md)|None|Deletes a [directorySetting](../resources/directorysetting.md).|
|[Update directorySetting](../api/directorysetting-update.md)|[directorySetting](../resources/directorySetting.md)|Update the properties of a [directorySetting](../resources/directorysetting.md) object.|
|[List settings](../api/group-list-settings.md)|[directorySetting](../resources/directorySetting.md) collection|Get the directorySettings from the settings navigation property.|
|[Add settings](../api/group-post-settings.md)|[directorySetting](../resources/directorySetting.md)|Add settings by posting to the settings collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|templateId|String||
|values|[settingValue](../resources/settingValue.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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


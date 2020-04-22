---
title: "groupSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# groupSetting resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupSettings](../api/groupsetting-list.md)|[groupSetting](../resources/groupsetting.md) collection|Get a list of the [groupSetting](../resources/groupsetting.md) objects and their properties.|
|[Get groupSetting](../api/groupsetting-get.md)|[groupSetting](../resources/groupsetting.md)|Read properties and relationships of a [groupSetting](../resources/groupsetting.md) object.|
|[Create groupSetting](../api/groupsetting-post-groupsettings.md)|[groupSetting](../resources/groupsetting.md)|Create a new [groupSetting](../resources/groupsetting.md) object.|
|[Delete groupSetting](../api/groupsetting-delete.md)|None|Deletes a [groupSetting](../resources/groupsetting.md).|
|[Update groupSetting](../api/groupsetting-update.md)|[groupSetting](../resources/groupsetting.md)|Update the properties of a [groupSetting](../resources/groupsetting.md) object.|
|[List settings](../api/group-list-settings.md)|[groupSetting](../resources/groupsetting.md) collection|Get the groupSettings from the settings navigation property.|
|[Create settings](../api/group-post-settings.md)|[groupSetting](../resources/groupsetting.md)|Create a new settings object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|templateId|String|**TODO: Add Description**|
|values|[settingValue](../resources/settingvalue.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupSetting",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupSetting",
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


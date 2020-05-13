---
title: "groupSetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupSetting resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groupSettings](../api/groupsetting-list.md)|[groupSetting](../resources/groupsetting.md) collection|Get a list of the [groupSetting](../resources/groupsetting.md) objects and their properties.|
|[Get groupSetting](../api/groupsetting-get.md)|[groupSetting](../resources/groupsetting.md)|Read the properties and relationships of a [groupSetting](../resources/groupsetting.md) object.|
|[Create groupSetting](../api/groupsetting-post-groupsettings.md)|[groupSetting](../resources/groupsetting.md)|Create a new [groupSetting](../resources/groupsetting.md) object.|
|[Delete groupSetting](../api/groupsetting-delete.md)|None|Deletes a [groupSetting](../resources/groupsetting.md) object.|
|[Update groupSetting](../api/groupsetting-update.md)|[groupSetting](../resources/groupsetting.md)|Update the properties of a [groupSetting](../resources/groupsetting.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|values|[settingValue](../resources/settingvalue.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupSetting",
  "baseType": "",
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


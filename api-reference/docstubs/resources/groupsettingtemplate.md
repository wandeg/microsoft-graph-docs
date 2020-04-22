---
title: "groupSettingTemplate resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# groupSettingTemplate resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List groupSettingTemplates](../api/groupsettingtemplate-list.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md) collection|Get a list of the [groupSettingTemplate](../resources/groupsettingtemplate.md) objects and their properties.|
|[Get groupSettingTemplate](../api/groupsettingtemplate-get.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md)|Read properties and relationships of a [groupSettingTemplate](../resources/groupsettingtemplate.md) object.|
|[Create groupSettingTemplate](../api/groupsettingtemplate-post-groupsettingtemplates.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md)|Create a new [groupSettingTemplate](../resources/groupsettingtemplate.md) object.|
|[Delete groupSettingTemplate](../api/groupsettingtemplate-delete.md)|None|Deletes a [groupSettingTemplate](../resources/groupsettingtemplate.md).|
|[Update groupSettingTemplate](../api/groupsettingtemplate-update.md)|[groupSettingTemplate](../resources/groupsettingtemplate.md)|Update the properties of a [groupSettingTemplate](../resources/groupsettingtemplate.md) object.|
|[checkMemberGroups](../api/groupsettingtemplate-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/groupsettingtemplate-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/groupsettingtemplate-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/groupsettingtemplate-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/groupsettingtemplate-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|values|[settingTemplateValue](../resources/settingtemplatevalue.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupSettingTemplate",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupSettingTemplate",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "values": [
    {
      "@odata.type": "microsoft.graph.settingTemplateValue"
    }
  ]
}
```


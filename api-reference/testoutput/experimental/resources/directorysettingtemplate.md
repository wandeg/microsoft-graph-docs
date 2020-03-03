---
title: "directorySettingTemplate resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# directorySettingTemplate resource type

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryObject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directorySettingTemplates](../api/directorysettingtemplate-list.md)|[directorySettingTemplate](../resources/directorySettingTemplate.md) collection|List properties and relationships of the [directorySettingTemplate](../resources/directorysettingtemplate.md) objects.|
|[Get directorySettingTemplate](../api/directorysettingtemplate-get.md)|[directorySettingTemplate](../resources/directorySettingTemplate.md)|Read properties and relationships of the [directorySettingTemplate](../resources/directorysettingtemplate.md) object.|
|[Create directorySettingTemplate](../api/directorysettingtemplate-post-directorysettingtemplates.md)|[directorySettingTemplate](../resources/directorySettingTemplate.md)|Create a new [directorySettingTemplate](../resources/directorysettingtemplate.md) object.|
|[Delete directorySettingTemplate](../api/directorysettingtemplate-delete.md)|None|Deletes a [directorySettingTemplate](../resources/directorysettingtemplate.md).|
|[Update directorySettingTemplate](../api/directorysettingtemplate-update.md)|[directorySettingTemplate](../resources/directorySettingTemplate.md)|Update the properties of a [directorySettingTemplate](../resources/directorysettingtemplate.md) object.|
|[checkMemberGroups](../api/directorysettingtemplate-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/directorysettingtemplate-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/directorysettingtemplate-getmembergroups.md)|String collection||
|[getMemberObjects](../api/directorysettingtemplate-getmemberobjects.md)|String collection||
|[restore](../api/directorysettingtemplate-restore.md)|[directoryObject](../resources/directoryObject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|description|String||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|values|[settingTemplateValue](../resources/settingTemplateValue.md) collection||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directorySettingTemplate",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directorySettingTemplate",
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


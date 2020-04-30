---
title: "directorySettingTemplate resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directorySettingTemplate resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directorySettingTemplates](../api/microsoft.directoryservices-directorysettingtemplate-list.md)|[directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md) collection|Get a list of the [directorySettingTemplate](../resources/directorysettingtemplate.md) objects and their properties.|
|[Get directorySettingTemplate](../api/microsoft.directoryservices-directorysettingtemplate-get.md)|[directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md)|Read properties and relationships of a [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md) object.|
|[Create directorySettingTemplate](../api/microsoft.directoryservices-directorysettingtemplate-post-directorysettingtemplates.md)|[directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md)|Create a new [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md) object.|
|[Delete directorySettingTemplate](../api/microsoft.directoryservices-directorysettingtemplate-delete.md)|None|Deletes a [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md).|
|[Update directorySettingTemplate](../api/microsoft.directoryservices-directorysettingtemplate-update.md)|[directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md)|Update the properties of a [directorySettingTemplate](../resources/microsoft.directoryservices-directorysettingtemplate.md) object.|
|[checkMemberGroups](../api/microsoft.directoryservices-directorysettingtemplate-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/microsoft.directoryservices-directorysettingtemplate-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/microsoft.directoryservices-directorysettingtemplate-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/microsoft.directoryservices-directorysettingtemplate-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/microsoft.directoryservices-directorysettingtemplate-restore.md)|[directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|values|[settingTemplateValue](../resources/microsoft.directoryservices-settingtemplatevalue.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.directorySettingTemplate",
  "baseType": "Microsoft.DirectoryServices.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.directorySettingTemplate",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "description": "String",
  "values": [
    {
      "@odata.type": "Microsoft.DirectoryServices.settingTemplateValue"
    }
  ]
}
```


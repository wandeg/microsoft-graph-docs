---
title: "directorySetting resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# directorySetting resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directorySettings](../api/microsoft.directoryservices-directorysetting-list.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md) collection|Get a list of the [directorySetting](../resources/directorysetting.md) objects and their properties.|
|[Get directorySetting](../api/microsoft.directoryservices-directorysetting-get.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md)|Read properties and relationships of a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.|
|[Create directorySetting](../api/microsoft.directoryservices-directorysetting-post-settings.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md)|Create a new [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.|
|[Delete directorySetting](../api/microsoft.directoryservices-directorysetting-delete.md)|None|Deletes a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md).|
|[Update directorySetting](../api/microsoft.directoryservices-directorysetting-update.md)|[directorySetting](../resources/microsoft.directoryservices-directorysetting.md)|Update the properties of a [directorySetting](../resources/microsoft.directoryservices-directorysetting.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|templateId|String|**TODO: Add Description**|
|values|[settingValue](../resources/microsoft.directoryservices-settingvalue.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.directorySetting",
  "baseType": "",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.directorySetting",
  "id": "String (identifier)",
  "displayName": "String",
  "templateId": "String",
  "values": [
    {
      "@odata.type": "Microsoft.DirectoryServices.settingValue"
    }
  ]
}
```


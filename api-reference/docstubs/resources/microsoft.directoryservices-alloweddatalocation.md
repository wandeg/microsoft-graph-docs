---
title: "allowedDataLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# allowedDataLocation resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List allowedDataLocations](../api/microsoft.directoryservices-alloweddatalocation-list.md)|[allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md) collection|Get a list of the [allowedDataLocation](../resources/alloweddatalocation.md) objects and their properties.|
|[Get allowedDataLocation](../api/microsoft.directoryservices-alloweddatalocation-get.md)|[allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md)|Read properties and relationships of an [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md) object.|
|[Create allowedDataLocation](../api/microsoft.directoryservices-alloweddatalocation-post-alloweddatalocations.md)|[allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md)|Create a new [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md) object.|
|[Delete allowedDataLocation](../api/microsoft.directoryservices-alloweddatalocation-delete.md)|None|Deletes an [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md).|
|[Update allowedDataLocation](../api/microsoft.directoryservices-alloweddatalocation-update.md)|[allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md)|Update the properties of a [allowedDataLocation](../resources/microsoft.directoryservices-alloweddatalocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appId|String|**TODO: Add Description**|
|domain|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|
|location|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "Microsoft.DirectoryServices.allowedDataLocation",
  "baseType": "",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.allowedDataLocation",
  "id": "String (identifier)",
  "appId": "String",
  "location": "String",
  "isDefault": true,
  "domain": "String"
}
```


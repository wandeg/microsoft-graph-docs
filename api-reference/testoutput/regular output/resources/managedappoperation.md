---
title: "managedAppOperation resource type"
description: "Represents an operation applied against an app registration."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# managedAppOperation resource type

Represents an operation applied against an app registration.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedAppOperation](../api/managedappoperation-get.md)|[managedAppOperation](../resources/managedAppOperation.md)|Read properties and relationships of the [managedAppOperation](../resources/managedappoperation.md) object.|
|[Delete managedAppOperation](../api/managedappoperation-delete.md)|None|Deletes a [managedAppOperation](../resources/managedappoperation.md).|
|[Update managedAppOperation](../api/managedappoperation-update.md)|[managedAppOperation](../resources/managedAppOperation.md)|Update the properties of a [managedAppOperation](../resources/managedappoperation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|The operation name.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|The last time the app operation was modified.|
|state|String|The current state of the operation|
|version|String|Version of the entity.|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```


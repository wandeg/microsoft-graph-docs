---
title: "administrativeUnit resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# administrativeUnit resource type

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryObject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List administrativeUnits](../api/administrativeunit-list.md)|[administrativeUnit](../resources/administrativeUnit.md) collection|List properties and relationships of the [administrativeUnit](../resources/administrativeunit.md) objects.|
|[Get administrativeUnit](../api/administrativeunit-get.md)|[administrativeUnit](../resources/administrativeUnit.md)|Read properties and relationships of the [administrativeUnit](../resources/administrativeunit.md) object.|
|[Create administrativeUnit](../api/administrativeunit-create.md)|[administrativeUnit](../resources/administrativeUnit.md)|Create a new [administrativeUnit](../resources/administrativeunit.md) object.|
|[Delete administrativeUnit](../api/administrativeunit-delete.md)|None|Deletes a [administrativeUnit](../resources/administrativeunit.md).|
|[Update administrativeUnit](../api/administrativeunit-update.md)|[administrativeUnit](../resources/administrativeUnit.md)|Update the properties of a [administrativeUnit](../resources/administrativeunit.md) object.|
|[checkMemberGroups](../api/administrativeunit-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/administrativeunit-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/administrativeunit-getmembergroups.md)|String collection||
|[getMemberObjects](../api/administrativeunit-getmemberobjects.md)|String collection||
|[restore](../api/administrativeunit-restore.md)|[directoryObject](../resources/directoryObject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryObject.md)|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.administrativeUnit",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.administrativeUnit",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)"
}
```


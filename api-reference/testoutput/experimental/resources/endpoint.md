---
title: "endpoint resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# endpoint resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List endpoints](../api/endpoint-list.md)|[endpoint](../resources/endpoint.md) collection|List properties and relationships of the [endpoint](../resources/endpoint.md) objects.|
|[Get endpoint](../api/endpoint-get.md)|[endpoint](../resources/endpoint.md)|Read properties and relationships of the [endpoint](../resources/endpoint.md) object.|
|[Create endpoint](../api/endpoint-create.md)|[endpoint](../resources/endpoint.md)|Create a new [endpoint](../resources/endpoint.md) object.|
|[Delete endpoint](../api/endpoint-delete.md)|None|Deletes a [endpoint](../resources/endpoint.md).|
|[Update endpoint](../api/endpoint-update.md)|[endpoint](../resources/endpoint.md)|Update the properties of a [endpoint](../resources/endpoint.md) object.|
|[checkMemberGroups](../api/endpoint-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/endpoint-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/endpoint-getmembergroups.md)|String collection||
|[getMemberObjects](../api/endpoint-getmemberobjects.md)|String collection||
|[restore](../api/endpoint-restore.md)|[directoryObject](../resources/directoryobject.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|capability|String||
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|providerId|String||
|providerName|String||
|providerResourceId|String||
|uri|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.endpoint",
  "baseType": "microsoft.graph.directoryObject",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.endpoint",
  "id": "String (identifier)",
  "deletedDateTime": "String (timestamp)",
  "capability": "String",
  "providerId": "String",
  "providerName": "String",
  "uri": "String",
  "providerResourceId": "String"
}
```


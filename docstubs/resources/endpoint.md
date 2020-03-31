---
title: "endpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# endpoint resource type


Namespace: microsoft.graph




Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get endpoint](../api/endpoint-get.md)|[endpoint](../resources/endpoint.md)|Read properties and relationships of the [endpoint](../resources/endpoint.md) object.|
|[Update endpoint](../api/endpoint-update.md)|[endpoint](../resources/endpoint.md)|Update the properties of a [endpoint](../resources/endpoint.md) object.|
|[checkMemberGroups](../api/endpoint-checkmembergroups.md)|String collection||
|[checkMemberObjects](../api/endpoint-checkmemberobjects.md)|String collection||
|[getMemberGroups](../api/endpoint-getmembergroups.md)|String collection||
|[getMemberObjects](../api/endpoint-getmemberobjects.md)|String collection||
|[restore](../api/endpoint-restore.md)|[directoryObject](../resources/directoryobject.md)||
|[List endpoints](../api/group-list-endpoints.md)|[endpoint](../resources/endpoint.md) collection|Get the endpoints from the endpoints navigation property.|
|[Add endpoints](../api/group-post-endpoints.md)|[endpoint](../resources/endpoint.md)|Add endpoints by posting to the endpoints collection.|

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

## JSON representation
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


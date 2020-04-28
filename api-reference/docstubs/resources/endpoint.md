---
title: "endpoint resource type"
description: "Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# endpoint resource type


Namespace: microsoft.graph

Represents an Azure Active Directory object. The directoryObject type is the base type for many other directory entity types.


Inherits from [directoryObject](../resources/directoryobject.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get endpoint](../api/endpoint-get.md)|[endpoint](../resources/endpoint.md)|Read the properties and relationships of an [endpoint](../resources/endpoint.md) object.|
|[Update endpoint](../api/endpoint-update.md)|[endpoint](../resources/endpoint.md)|Update the properties of an [endpoint](../resources/endpoint.md) object.|
|[checkMemberGroups](../api/endpoint-checkmembergroups.md)|String collection|**TODO: Add Description**|
|[checkMemberObjects](../api/endpoint-checkmemberobjects.md)|String collection|**TODO: Add Description**|
|[getMemberGroups](../api/endpoint-getmembergroups.md)|String collection|**TODO: Add Description**|
|[getMemberObjects](../api/endpoint-getmemberobjects.md)|String collection|**TODO: Add Description**|
|[restore](../api/endpoint-restore.md)|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|capability|String|**TODO: Add Description**|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|providerId|String|**TODO: Add Description**|
|providerName|String|**TODO: Add Description**|
|providerResourceId|String|**TODO: Add Description**|
|uri|String|**TODO: Add Description**|

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


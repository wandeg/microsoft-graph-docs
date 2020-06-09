---
title: "ipNamedLocation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# ipNamedLocation resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [namedLocation](../resources/namedlocation.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List ipNamedLocations](../api/ipnamedlocation-list.md)|[ipNamedLocation](../resources/ipnamedlocation.md) collection|Get a list of the [ipNamedLocation](../resources/ipnamedlocation.md) objects and their properties.|
|[Create ipNamedLocation](../api/ipnamedlocation-create.md)|[ipNamedLocation](../resources/ipnamedlocation.md)|Create a new [ipNamedLocation](../resources/ipnamedlocation.md) object.|
|[Get ipNamedLocation](../api/ipnamedlocation-get.md)|[ipNamedLocation](../resources/ipnamedlocation.md)|Read the properties and relationships of an [ipNamedLocation](../resources/ipnamedlocation.md) object.|
|[Update ipNamedLocation](../api/ipnamedlocation-update.md)|[ipNamedLocation](../resources/ipnamedlocation.md)|Update the properties of an [ipNamedLocation](../resources/ipnamedlocation.md) object.|
|[Delete ipNamedLocation](../api/ipnamedlocation-delete.md)|None|Deletes an [ipNamedLocation](../resources/ipnamedlocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|displayName|String|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|ipRanges|[ipRange](../resources/intune-iprange.md) collection|**TODO: Add Description**|
|isTrusted|Boolean|**TODO: Add Description**|
|modifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [namedLocation](../resources/namedlocation.md)|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ipNamedLocation",
  "baseType": "microsoft.graph.namedLocation",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ipNamedLocation",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "ipRanges": [
    {
      "@odata.type": "microsoft.graph.iPv4CidrRange"
    }
  ],
  "isTrusted": "Boolean"
}
```


---
title: "ipNamedLocation resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# ipNamedLocation resource type




Inherits from [namedLocation](../resources/namedLocation.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List ipNamedLocations](../api/ipnamedlocation-list.md)|[ipNamedLocation](../resources/ipNamedLocation.md) collection|List properties and relationships of the [ipNamedLocation](../resources/ipnamedlocation.md) objects.|
|[Get ipNamedLocation](../api/ipnamedlocation-get.md)|[ipNamedLocation](../resources/ipNamedLocation.md)|Read properties and relationships of the [ipNamedLocation](../resources/ipnamedlocation.md) object.|
|[Create ipNamedLocation](../api/ipnamedlocation-create.md)|[ipNamedLocation](../resources/ipNamedLocation.md)|Create a new [ipNamedLocation](../resources/ipnamedlocation.md) object.|
|[Delete ipNamedLocation](../api/ipnamedlocation-delete.md)|None|Deletes a [ipNamedLocation](../resources/ipnamedlocation.md).|
|[Update ipNamedLocation](../api/ipnamedlocation-update.md)|[ipNamedLocation](../resources/ipNamedLocation.md)|Update the properties of a [ipNamedLocation](../resources/ipnamedlocation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|
|displayName|String| Inherited from [namedLocation](../resources/namedLocation.md)|
|id|String| Inherited from [entity](../resources/entity.md)|
|ipRanges|[ipRange](../resources/ipRange.md) collection||
|isTrusted|Boolean||
|modifiedDateTime|DateTimeOffset| Inherited from [namedLocation](../resources/namedLocation.md)|

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
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
  "isTrusted": true
}
```


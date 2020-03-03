---
title: "baseItemVersion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# baseItemVersion resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List baseItemVersions](../api/baseitemversion-list.md)|[baseItemVersion](../resources/baseItemVersion.md) collection|List properties and relationships of the [baseItemVersion](../resources/baseitemversion.md) objects.|
|[Get baseItemVersion](../api/baseitemversion-get.md)|[baseItemVersion](../resources/baseItemVersion.md)|Read properties and relationships of the [baseItemVersion](../resources/baseitemversion.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)||
|lastModifiedDateTime|DateTimeOffset||
|publication|[publicationFacet](../resources/publicationFacet.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.baseItemVersion",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  }
}
```


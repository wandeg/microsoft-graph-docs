---
title: "driveItemVersion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# driveItemVersion resource type




Inherits from [baseItemVersion](../resources/baseItemVersion.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get driveItemVersion](../api/driveitemversion-get.md)|[driveItemVersion](../resources/driveItemVersion.md)|Read properties and relationships of the [driveItemVersion](../resources/driveitemversion.md) object.|
|[Delete driveItemVersion](../api/driveitemversion-delete.md)|None|Deletes a [driveItemVersion](../resources/driveitemversion.md).|
|[Update driveItemVersion](../api/driveitemversion-update.md)|[driveItemVersion](../resources/driveItemVersion.md)|Update the properties of a [driveItemVersion](../resources/driveitemversion.md) object.|
|[restoreVersion](../api/driveitemversion-restoreversion.md)|None||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|content|Stream||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItemVersion](../resources/baseItemVersion.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItemVersion](../resources/baseItemVersion.md)|
|publication|[publicationFacet](../resources/publicationFacet.md)| Inherited from [baseItemVersion](../resources/baseItemVersion.md)|
|size|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "baseType": "microsoft.graph.baseItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.driveItemVersion",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet"
  },
  "content": "Stream",
  "size": 1024
}
```


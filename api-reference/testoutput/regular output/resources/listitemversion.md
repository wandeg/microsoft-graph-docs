---
title: "listItemVersion resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# listItemVersion resource type




Inherits from [baseItemVersion](../resources/baseItemVersion.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get listItemVersion](../api/listitemversion-get.md)|[listItemVersion](../resources/listItemVersion.md)|Read properties and relationships of the [listItemVersion](../resources/listitemversion.md) object.|
|[Delete listItemVersion](../api/listitemversion-delete.md)|None|Deletes a [listItemVersion](../resources/listitemversion.md).|
|[Update listItemVersion](../api/listitemversion-update.md)|[listItemVersion](../resources/listItemVersion.md)|Update the properties of a [listItemVersion](../resources/listitemversion.md) object.|
|[restoreVersion](../api/listitemversion-restoreversion.md)|None||
|[Get fieldValueSet](../api/fieldvalueset-get.md)|[fieldValueSet](../resources/fieldValueSet.md)|Read properties and relationships of the [fieldValueSet](../resources/fieldvalueset.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identitySet.md)| Inherited from [baseItemVersion](../resources/baseItemVersion.md)|
|lastModifiedDateTime|DateTimeOffset| Inherited from [baseItemVersion](../resources/baseItemVersion.md)|
|publication|[publicationFacet](../resources/publicationFacet.md)| Inherited from [baseItemVersion](../resources/baseItemVersion.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|fields|[fieldValueSet](../resources/fieldValueSet.md)||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.listItemVersion",
  "baseType": "microsoft.graph.baseItemVersion",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.listItemVersion",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "String",
      "id": "String"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "lastModifiedDateTime": "String (timestamp)",
  "publication": {
    "@odata.type": "microsoft.graph.publicationFacet",
    "level": "String",
    "versionId": "String"
  }
}
```


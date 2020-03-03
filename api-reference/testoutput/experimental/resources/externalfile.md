---
title: "externalFile resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# externalFile resource type




Inherits from [externalItem](../resources/externalItem.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List externalFiles](../api/externalfile-list.md)|[externalFile](../resources/externalFile.md) collection|List properties and relationships of the [externalFile](../resources/externalfile.md) objects.|
|[Get externalFile](../api/externalfile-get.md)|[externalFile](../resources/externalFile.md)|Read properties and relationships of the [externalFile](../resources/externalfile.md) object.|
|[Create externalFile](../api/externalfile-create.md)|[externalFile](../resources/externalFile.md)|Create a new [externalFile](../resources/externalfile.md) object.|
|[Delete externalFile](../api/externalfile-delete.md)|None|Deletes a [externalFile](../resources/externalfile.md).|
|[Update externalFile](../api/externalfile-update.md)|[externalFile](../resources/externalFile.md)|Update the properties of a [externalFile](../resources/externalfile.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acl|[acl](../resources/acl.md) collection| Inherited from [externalItem](../resources/externalItem.md)|
|content|String| Inherited from [externalItem](../resources/externalItem.md)|
|createdBy|String||
|createdDateTime|DateTimeOffset||
|extension|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|String||
|modifiedDateTime|DateTimeOffset||
|name|String||
|properties|[properties](../resources/properties.md)| Inherited from [externalItem](../resources/externalItem.md)|
|size|Int64||
|title|String||
|url|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalFile",
  "baseType": "microsoft.graph.externalItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.externalFile",
  "id": "String (identifier)",
  "properties": {
    "@odata.type": "microsoft.graph.properties"
  },
  "content": "String",
  "acl": [
    {
      "@odata.type": "microsoft.graph.acl"
    }
  ],
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "createdBy": "String",
  "lastModifiedBy": "String",
  "title": "String",
  "url": "String",
  "name": "String",
  "extension": "String",
  "size": 1024
}
```


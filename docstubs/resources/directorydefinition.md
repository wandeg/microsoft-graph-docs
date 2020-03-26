---
title: "directoryDefinition resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# directoryDefinition resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List directoryDefinitions](../api/directorydefinition-list.md)|[directoryDefinition](../resources/directorydefinition.md) collection|List properties and relationships of the [directoryDefinition](../resources/directorydefinition.md) objects.|
|[Get directoryDefinition](../api/directorydefinition-get.md)|[directoryDefinition](../resources/directorydefinition.md)|Read properties and relationships of the [directoryDefinition](../resources/directorydefinition.md) object.|
|[Create directoryDefinition](../api/directorydefinition-post-directories.md)|[directoryDefinition](../resources/directorydefinition.md)|Create a new [directoryDefinition](../resources/directorydefinition.md) object.|
|[Delete directoryDefinition](../api/directorydefinition-delete.md)|None|Deletes a [directoryDefinition](../resources/directorydefinition.md).|
|[Update directoryDefinition](../api/directorydefinition-update.md)|[directoryDefinition](../resources/directorydefinition.md)|Update the properties of a [directoryDefinition](../resources/directorydefinition.md) object.|
|[discover](../api/directorydefinition-discover.md)|[directoryDefinition](../resources/directorydefinition.md)||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|discoverabilities|Enumeration|. Possible values are: `None`, `AttributeNames`, `AttributeDataTypes`, `AttributeReadOnly`, `ReferenceAttributes`, `UnknownFutureValue`.|
|discoveryDateTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|name|String||
|objects|[objectDefinition](../resources/objectdefinition.md) collection||
|readOnly|Boolean||
|version|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.directoryDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.directoryDefinition",
  "id": "String (identifier)",
  "discoveryDateTime": "String (timestamp)",
  "discoverabilities": "String",
  "name": "String",
  "objects": [
    {
      "@odata.type": "microsoft.graph.objectDefinition"
    }
  ],
  "readOnly": true,
  "version": "String"
}
```


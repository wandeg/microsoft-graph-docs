---
title: "office365ActivationCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# office365ActivationCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365ActivationCountses](../api/office365activationcounts-list.md)|[office365ActivationCounts](../resources/office365ActivationCounts.md) collection|List properties and relationships of the [office365ActivationCounts](../resources/office365activationcounts.md) objects.|
|[Get office365ActivationCounts](../api/office365activationcounts-get.md)|[office365ActivationCounts](../resources/office365ActivationCounts.md)|Read properties and relationships of the [office365ActivationCounts](../resources/office365activationcounts.md) object.|
|[Create office365ActivationCounts](../api/office365activationcounts-create.md)|[office365ActivationCounts](../resources/office365ActivationCounts.md)|Create a new [office365ActivationCounts](../resources/office365activationcounts.md) object.|
|[Delete office365ActivationCounts](../api/office365activationcounts-delete.md)|None|Deletes a [office365ActivationCounts](../resources/office365activationcounts.md).|
|[Update office365ActivationCounts](../api/office365activationcounts-update.md)|[office365ActivationCounts](../resources/office365ActivationCounts.md)|Update the properties of a [office365ActivationCounts](../resources/office365activationcounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|android|Int64||
|id|String| Inherited from [entity](../resources/entity.md)|
|ios|Int64||
|mac|Int64||
|productType|String||
|reportRefreshDate|Date||
|windows|Int64||
|windows10Mobile|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365ActivationCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365ActivationCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "productType": "String",
  "windows": 1024,
  "mac": 1024,
  "android": 1024,
  "ios": 1024,
  "windows10Mobile": 1024
}
```


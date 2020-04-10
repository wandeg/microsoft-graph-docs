---
title: "printServiceEndpoint resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printServiceEndpoint resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get printServiceEndpoint](../api/printserviceendpoint-get.md)|[printServiceEndpoint](../resources/printserviceendpoint.md)|Read properties and relationships of the [printServiceEndpoint](../resources/printserviceendpoint.md) object.|
|[Update printServiceEndpoint](../api/printserviceendpoint-update.md)|[printServiceEndpoint](../resources/printserviceendpoint.md)|Update the properties of a [printServiceEndpoint](../resources/printserviceendpoint.md) object.|
|[List endpoints](../api/printservice-list-endpoints.md)|[printServiceEndpoint](../resources/printserviceendpoint.md) collection|Get the printServiceEndpoints from the endpoints navigation property.|
|[Add endpoints](../api/printservice-post-endpoints.md)|[printServiceEndpoint](../resources/printserviceendpoint.md)|Add endpoints by posting to the endpoints collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|uri|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printServiceEndpoint",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printServiceEndpoint",
  "id": "String (identifier)",
  "displayName": "String",
  "uri": "String"
}
```


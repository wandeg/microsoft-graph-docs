---
title: "inferenceClassificationOverride resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# inferenceClassificationOverride resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get inferenceClassificationOverride](../api/inferenceclassificationoverride-get.md)|[inferenceClassificationOverride](../resources/inferenceClassificationOverride.md)|Read properties and relationships of the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|
|[Delete inferenceClassificationOverride](../api/inferenceclassificationoverride-delete.md)|None|Deletes a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).|
|[Update inferenceClassificationOverride](../api/inferenceclassificationoverride-update.md)|[inferenceClassificationOverride](../resources/inferenceClassificationOverride.md)|Update the properties of a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classifyAs|Enumeration|. Possible values are: `focused`, `other`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|senderEmailAddress|[emailAddress](../resources/emailAddress.md)||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.inferenceClassificationOverride",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.inferenceClassificationOverride",
  "id": "String (identifier)",
  "classifyAs": "String",
  "senderEmailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  }
}
```


---
title: "inferenceClassificationOverride resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# inferenceClassificationOverride resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List inferenceClassificationOverrides](../api/inferenceclassificationoverride-list.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection|List properties and relationships of the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) objects.|
|[Get inferenceClassificationOverride](../api/inferenceclassificationoverride-get.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Read properties and relationships of the [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|
|[Create inferenceClassificationOverride](../api/inferenceclassificationoverride-create.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Create a new [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|
|[Delete inferenceClassificationOverride](../api/inferenceclassificationoverride-delete.md)|None|Deletes a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md).|
|[Update inferenceClassificationOverride](../api/inferenceclassificationoverride-update.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Update the properties of a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classifyAs|Enumeration|. Possible values are: `focused`, `other`.|
|id|String| Inherited from [entity](../resources/entity.md)|
|senderEmailAddress|[emailAddress](../resources/emailaddress.md)||

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


---
title: "inferenceClassificationOverride resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# inferenceClassificationOverride resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get inferenceClassificationOverride](../api/inferenceclassificationoverride-get.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Read properties and relationships of an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|
|[Update inferenceClassificationOverride](../api/inferenceclassificationoverride-update.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Update the properties of a [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) object.|
|[List overrides](../api/inferenceclassification-list-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) collection|Get the inferenceClassificationOverrides from the overrides navigation property.|
|[Create overrides](../api/inferenceclassification-post-overrides.md)|[inferenceClassificationOverride](../resources/inferenceclassificationoverride.md)|Create a new overrides object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classifyAs|inferenceClassificationType|**TODO: Add Description**. Possible values are: `focused`, `other`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|senderEmailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|

## Relationships
None

## JSON representation
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


---
title: "educationOutcome resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# educationOutcome resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get educationOutcome](../api/educationoutcome-get.md)|[educationOutcome](../resources/educationoutcome.md)|Read properties and relationships of the [educationOutcome](../resources/educationoutcome.md) object.|
|[List outcomes](../api/educationsubmission-list-outcomes.md)|[educationOutcome](../resources/educationoutcome.md) collection|Get the educationOutcomes from the outcomes navigation property.|
|[Add outcomes](../api/educationsubmission-post-outcomes.md)|[educationOutcome](../resources/educationoutcome.md)|Add outcomes by posting to the outcomes collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)||
|lastModifiedDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationOutcome",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationOutcome",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```


---
title: "userExperienceAnalyticsScoreHistory resource type"
description: "The user experience analytics device startup score history."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsScoreHistory resource type


Namespace: microsoft.graph

The user experience analytics device startup score history.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsScoreHistory](../api/userexperienceanalyticsscorehistory-get.md)|[userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md)|Read the properties and relationships of a [userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) object.|
|[Update userExperienceAnalyticsScoreHistory](../api/userexperienceanalyticsscorehistory-update.md)|[userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md)|Update the properties of a [userExperienceAnalyticsScoreHistory](../resources/userexperienceanalyticsscorehistory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|startupDateTime|DateTimeOffset|The user experience analytics device startup date time.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsScoreHistory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)"
}
```


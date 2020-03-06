---
title: "userExperienceAnalyticsOverview resource type"
description: "The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsOverview resource type


Namespace: microsoft.graph

The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[Update userExperienceAnalyticsOverview](../api/userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md)|Update the properties of a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|insights|[userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|The user experience analytics insights.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsOverview",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsOverview",
  "id": "String (identifier)",
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
    }
  ]
}
```


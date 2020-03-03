---
title: "userExperienceAnalyticsOverview resource type"
description: "The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# userExperienceAnalyticsOverview resource type

The user experience analytics overview entity contains the overall score and the scores and insights of every metric of all categories.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List userExperienceAnalyticsOverviews](../api/intune-devices-userexperienceanalyticsoverview-list.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md) collection|List properties and relationships of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) objects.|
|[Get userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-get.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|Read properties and relationships of the [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[Create userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-create.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|Create a new [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|
|[Delete userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-delete.md)|None|Deletes a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md).|
|[Update userExperienceAnalyticsOverview](../api/intune-devices-userexperienceanalyticsoverview-update.md)|[userExperienceAnalyticsOverview](../resources/intune-devices-userExperienceAnalyticsOverview.md)|Update the properties of a [userExperienceAnalyticsOverview](../resources/userexperienceanalyticsoverview.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|insights|[userExperienceAnalyticsInsight](../resources/intune-devices-userExperienceAnalyticsInsight.md) collection|The user experience analytics insights.|

## Relationships
None

## JSON Representation
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


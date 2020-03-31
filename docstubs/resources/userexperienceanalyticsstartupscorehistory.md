---
title: "userExperienceAnalyticsStartupScoreHistory resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsStartupScoreHistory resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsStartupScoreHistory](../api/userexperienceanalyticsstartupscorehistory-get.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md)|Read properties and relationships of the [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) object.|
|[Update userExperienceAnalyticsStartupScoreHistory](../api/userexperienceanalyticsstartupscorehistory-update.md)|[userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md)|Update the properties of a [userExperienceAnalyticsStartupScoreHistory](../resources/userexperienceanalyticsstartupscorehistory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|startupDateTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsStartupScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)"
}
```


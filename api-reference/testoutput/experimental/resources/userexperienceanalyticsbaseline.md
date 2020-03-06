---
title: "userExperienceAnalyticsBaseline resource type"
description: "The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userExperienceAnalyticsBaseline resource type


Namespace: microsoft.graph

The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get userExperienceAnalyticsBaseline](../api/userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Read properties and relationships of the [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[Update userExperienceAnalyticsBaseline](../api/userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Update the properties of a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[Get userExperienceAnalyticsCategory](../api/userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|
|[Get userExperienceAnalyticsCategory](../api/userexperienceanalyticscategory-get.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Read properties and relationships of the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date the custom baseline was created.|
|displayName|String|The name of the user experience analytics baseline.|
|id|String| Inherited from [entity](../resources/entity.md)|
|isBuiltIn|Boolean|Signifies if the current baseline is the commercial median baseline or a custom baseline.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics best practices metrics.|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics device boot performance metrics.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "displayName": "String",
  "isBuiltIn": true,
  "createdDateTime": "String (timestamp)"
}
```


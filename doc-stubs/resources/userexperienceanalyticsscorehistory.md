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

## Properties
|Property|Type|Description|
|:---|:---|:---|
|coreBootScore|Int32|The user experience analytics device core boot score.|
|coreSigninScore|Int32|The User experience analytics device core sign-in score.|
|id|String|The unique identifier of the user experience analytics device startup process.|
|recommendedSoftwareScore|Int32|The User experience analytics device core sign-in score.|
|startupDateTime|DateTimeOffset|The user experience analytics device startup date time.|
|startupScore|Int32|User experience analytics device startup score.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsScoreHistory",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsScoreHistory",
  "id": "String (identifier)",
  "startupDateTime": "String (timestamp)",
  "startupScore": "Integer",
  "coreBootScore": "Integer",
  "coreSigninScore": "Integer",
  "recommendedSoftwareScore": "Integer"
}
```


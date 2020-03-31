---
title: "adminConsent resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# adminConsent resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|shareAPNSData|Enumeration| Possible values are: `notConfigured`, `granted`, `notGranted`.|
|shareUserExperienceAnalyticsData|Enumeration| Possible values are: `notConfigured`, `granted`, `notGranted`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```


---
title: "adminConsent resource type"
description: "Admin consent information."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# adminConsent resource type


Namespace: microsoft.graph

Admin consent information.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|shareAPNSData|adminConsentState|The admin consent state of sharing user and device data to Apple. Possible values are: `notConfigured`, `granted`, `notGranted`.|
|shareUserExperienceAnalyticsData|adminConsentState|Gets or sets the admin consent for sharing User experience analytics data. Possible values are: `notConfigured`, `granted`, `notGranted`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.adminConsent",
  "shareAPNSData": "String",
  "shareUserExperienceAnalyticsData": "String"
}
```


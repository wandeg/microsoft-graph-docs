---
title: "adminConsent resource type"
description: "Admin consent information."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# adminConsent resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Admin consent information.

## Properties

| Property                         | Type   | Description                                                                |
| :------------------------------- | :----- | :------------------------------------------------------------------------- |
| shareAPNSData                    | String | The admin consent state of sharing user and device data to Apple.          |
| shareUserExperienceAnalyticsData | String | Gets or sets the admin consent for sharing User experience analytics data. |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "notConfigured | granted | notGranted",
  "shareUserExperienceAnalyticsData": "notConfigured | granted | notGranted"
}
```
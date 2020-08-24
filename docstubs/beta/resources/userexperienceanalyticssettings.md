---
title: "userExperienceAnalyticsSettings resource type"
description: "The user experience analytics insight is the recomendation to improve the user experience analytics score."
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# userExperienceAnalyticsSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics insight is the recomendation to improve the user experience analytics score.

## Properties

| Property                                    | Type    | Description                                                                                                         |
| :------------------------------------------ | :------ | :------------------------------------------------------------------------------------------------------------------ |
| configurationManagerDataConnectorConfigured | Boolean | True if Tenant attach is configured. If configured then SCCM tenant attached devices will show up in UXA reporting. |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsSettings",
  "configurationManagerDataConnectorConfigured": "Boolean"
}
```
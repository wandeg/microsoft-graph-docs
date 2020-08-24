---
title: "configurationManagerClientEnabledFeatures resource type"
description: "configuration Manager client enabled features"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# configurationManagerClientEnabledFeatures resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

configuration Manager client enabled features

## Properties

| Property                 | Type    | Description                                              |
| :----------------------- | :------ | :------------------------------------------------------- |
| compliancePolicy         | Boolean | Whether compliance policy is managed by Intune           |
| deviceConfiguration      | Boolean | Whether device configuration is managed by Intune        |
| endpointProtection       | Boolean | Whether Endpoint Protection is managed by Intune         |
| inventory                | Boolean | Whether inventory is managed by Intune                   |
| modernApps               | Boolean | Whether modern application is managed by Intune          |
| officeApps               | Boolean | Whether Office application is managed by Intune          |
| resourceAccess           | Boolean | Whether resource access is managed by Intune             |
| windowsUpdateForBusiness | Boolean | Whether Windows Update for Business is managed by Intune |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "compliancePolicy": "Boolean",
  "deviceConfiguration": "Boolean",
  "endpointProtection": "Boolean",
  "inventory": "Boolean",
  "modernApps": "Boolean",
  "officeApps": "Boolean",
  "resourceAccess": "Boolean",
  "windowsUpdateForBusiness": "Boolean"
}
```
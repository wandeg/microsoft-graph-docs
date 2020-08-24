---
title: "comanagementEligibleDevicesSummary resource type"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: "resourcePageType"
---

# comanagementEligibleDevicesSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## Properties

| Property                         | Type  | Description                                                                              |
| :------------------------------- | :---- | :--------------------------------------------------------------------------------------- |
| comanagedCount                   | Int32 | Count of devices already Co-Managed                                                      |
| eligibleButNotAzureAdJoinedCount | Int32 | Count of devices eligible for Co-Management but not yet joined to Azure Active Directory |
| eligibleCount                    | Int32 | Count of devices fully eligible for Co-Management                                        |
| ineligibleCount                  | Int32 | Count of devices ineligible for Co-Management                                            |
| needsOsUpdateCount               | Int32 | Count of devices that will be eligible for Co-Management after an OS update              |

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.comanagementEligibleDevicesSummary",
}
-->

```json
{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevicesSummary",
  "comanagedCount": "Int32",
  "eligibleButNotAzureAdJoinedCount": "Int32",
  "eligibleCount": "Int32",
  "ineligibleCount": "Int32",
  "needsOsUpdateCount": "Int32"
}
```
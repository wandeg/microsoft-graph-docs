---
title: "overallPrintUsageSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# overallPrintUsageSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activePrintersCount|Int32|**TODO: Add Description**|
|activeUsersCount|Int32|**TODO: Add Description**|
|daysInPeriod|Int32|**TODO: Add Description**|
|topPrinters|[printerUsageSummary](../resources/printerusagesummary.md) collection|**TODO: Add Description**|
|topUsers|[userPrintUsageSummary](../resources/userprintusagesummary.md) collection|**TODO: Add Description**|
|totalIncompleteJobs|Int32|**TODO: Add Description**|
|totalJobsProcessed|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.overallPrintUsageSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.overallPrintUsageSummary",
  "topUsers": [
    {
      "@odata.type": "microsoft.graph.userPrintUsageSummary"
    }
  ],
  "topPrinters": [
    {
      "@odata.type": "microsoft.graph.printerUsageSummary"
    }
  ],
  "daysInPeriod": "Integer",
  "activeUsersCount": "Integer",
  "activePrintersCount": "Integer",
  "totalJobsProcessed": "Integer",
  "totalIncompleteJobs": "Integer"
}
```


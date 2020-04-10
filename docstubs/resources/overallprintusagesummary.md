---
title: "overallPrintUsageSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# overallPrintUsageSummary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|activePrintersCount|Int32||
|activeUsersCount|Int32||
|daysInPeriod|Int32||
|topPrinters|[printerUsageSummary](../resources/printerusagesummary.md) collection||
|topUsers|[userPrintUsageSummary](../resources/userprintusagesummary.md) collection||
|totalIncompleteJobs|Int32||
|totalJobsProcessed|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.userPrintUsageSummary",
      "userPrincipalName": "String",
      "userDisplayName": "String",
      "completedJobCount": 1024,
      "incompleteJobCount": 1024,
      "user": {
        "@odata.type": "microsoft.graph.identity",
        "id": "String",
        "displayName": "String"
      }
    }
  ],
  "topPrinters": [
    {
      "@odata.type": "microsoft.graph.printerUsageSummary",
      "printerId": "String",
      "printerDisplayName": "String",
      "printerManufacturer": "String",
      "printerModel": "String",
      "printer": {
        "@odata.type": "#microsoft.graph.directoryObject",
        "id": "String (identifier)",
        "deletedDateTime": "String (timestamp)"
      }
    }
  ],
  "daysInPeriod": 1024,
  "activeUsersCount": 1024,
  "activePrintersCount": 1024,
  "totalJobsProcessed": 1024,
  "totalIncompleteJobs": 1024
}
```


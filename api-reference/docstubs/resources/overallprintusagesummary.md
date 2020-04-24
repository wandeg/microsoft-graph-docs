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


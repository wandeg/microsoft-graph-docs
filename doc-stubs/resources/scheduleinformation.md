---
title: "scheduleInformation resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# scheduleInformation resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|availabilityView|String|**TODO: Add Description**|
|error|[freeBusyError](../resources/freebusyerror.md)|**TODO: Add Description**|
|scheduleId|String|**TODO: Add Description**|
|scheduleItems|[scheduleItem](../resources/scheduleitem.md) collection|**TODO: Add Description**|
|workingHours|[workingHours](../resources/workinghours.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.scheduleInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.scheduleInformation",
  "scheduleId": "String",
  "scheduleItems": [
    {
      "@odata.type": "microsoft.graph.scheduleItem"
    }
  ],
  "availabilityView": "String",
  "error": {
    "@odata.type": "microsoft.graph.freeBusyError"
  },
  "workingHours": {
    "@odata.type": "microsoft.graph.workingHours"
  }
}
```


---
title: "printerUsageSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# printerUsageSummary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedJobCount|Int32||
|incompleteJobCount|Int32||
|printer|[directoryObject](../resources/directoryobject.md)||
|printerDisplayName|String||
|printerId|String||
|printerManufacturer|String||
|printerModel|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.printerUsageSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printerUsageSummary",
  "printerId": "String",
  "printerDisplayName": "String",
  "printerManufacturer": "String",
  "printerModel": "String",
  "completedJobCount": 1024,
  "incompleteJobCount": 1024,
  "printer": {
    "@odata.type": "#microsoft.graph.directoryObject",
    "id": "String (identifier)",
    "deletedDateTime": "String (timestamp)"
  }
}
```


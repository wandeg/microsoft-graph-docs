---
title: "printerUsageSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printerUsageSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedJobCount|Int32|**TODO: Add Description**|
|incompleteJobCount|Int32|**TODO: Add Description**|
|printer|[directoryObject](../resources/directoryobject.md)|**TODO: Add Description**|
|printerDisplayName|String|**TODO: Add Description**|
|printerId|String|**TODO: Add Description**|
|printerManufacturer|String|**TODO: Add Description**|
|printerModel|String|**TODO: Add Description**|

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


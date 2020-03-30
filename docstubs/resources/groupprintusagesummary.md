---
title: "groupPrintUsageSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# groupPrintUsageSummary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedJobCount|Int32||
|group|[identity](../resources/identity.md)||
|groupDisplayName|String||
|groupMail|String||
|incompleteJobCount|Int32||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPrintUsageSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPrintUsageSummary",
  "groupMail": "String",
  "groupDisplayName": "String",
  "completedJobCount": 1024,
  "incompleteJobCount": 1024,
  "group": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  }
}
```


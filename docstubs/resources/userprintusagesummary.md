---
title: "userPrintUsageSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# userPrintUsageSummary resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedJobCount|Int32||
|incompleteJobCount|Int32||
|user|[identity](../resources/identity.md)||
|userDisplayName|String||
|userPrincipalName|String||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userPrintUsageSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userPrintUsageSummary",
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
```


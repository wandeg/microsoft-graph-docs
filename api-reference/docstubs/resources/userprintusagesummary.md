---
title: "userPrintUsageSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userPrintUsageSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|completedJobCount|Int32|**TODO: Add Description**|
|incompleteJobCount|Int32|**TODO: Add Description**|
|user|[identity](../resources/identity.md)|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|

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


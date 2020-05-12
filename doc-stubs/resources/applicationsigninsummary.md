---
title: "applicationSignInSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# applicationSignInSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|failedSignInCount|Int64|**TODO: Add Description**|
|successfulSignInCount|Int64|**TODO: Add Description**|
|successPercentage|Double|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.applicationSignInSummary",
  "baseType": "",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.applicationSignInSummary",
  "appId": "String",
  "appDisplayName": "String",
  "successfulSignInCount": "Integer",
  "failedSignInCount": "Integer",
  "successPercentage": "Double"
}
```


---
title: "userAccount resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userAccount resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|service|String|**TODO: Add Description**|
|signinName|String|**TODO: Add Description**|
|status|accountStatus|**TODO: Add Description**. Possible values are: `unknown`, `staged`, `active`, `suspended`, `deleted`, `unknownFutureValue`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userAccount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAccount",
  "displayName": "String",
  "lastSeenDateTime": "String (timestamp)",
  "riskScore": "String",
  "service": "String",
  "signinName": "String",
  "status": "String"
}
```


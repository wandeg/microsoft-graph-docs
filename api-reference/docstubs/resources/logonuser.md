---
title: "logonUser resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# logonUser resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountDomain|String|**TODO: Add Description**|
|accountName|String|**TODO: Add Description**|
|accountType|userAccountSecurityType|**TODO: Add Description**. Possible values are: `unknown`, `standard`, `power`, `administrator`, `unknownFutureValue`.|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|logonId|String|**TODO: Add Description**|
|logonTypes|logonType collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.logonUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.logonUser",
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": [
    "String"
  ]
}
```


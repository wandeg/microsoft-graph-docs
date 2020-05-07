---
title: "loggedOnUser resource type"
description: "Logged On User"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# loggedOnUser resource type


Namespace: microsoft.graph

Logged On User

## Properties
|Property|Type|Description|
|:---|:---|:---|
|lastLogOnDateTime|DateTimeOffset|Date time when user logs on|
|userId|String|User id|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.management.services.api.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.management.services.api.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```


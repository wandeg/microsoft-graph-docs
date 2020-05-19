---
title: "incomingContext resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# incomingContext resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|observedParticipantId|String|**TODO: Add Description**|
|onBehalfOf|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|sourceParticipantId|String|**TODO: Add Description**|
|transferor|[identitySet](../resources/identityset.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.incomingContext"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.incomingContext",
  "sourceParticipantId": "String",
  "observedParticipantId": "String",
  "onBehalfOf": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "transferor": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


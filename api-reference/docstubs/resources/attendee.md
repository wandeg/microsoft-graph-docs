---
title: "attendee resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# attendee resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [attendeeBase](../resources/attendeebase.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description** Inherited from [recipient](../resources/recipient.md)|
|status|[responseStatus](../resources/responsestatus.md)|**TODO: Add Description**|
|type|attendeeType|**TODO: Add Description** Inherited from [attendeeBase](../resources/attendeebase.md). Possible values are: `required`, `optional`, `resource`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendee"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendee",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "String",
    "address": "String"
  },
  "type": "String",
  "status": {
    "@odata.type": "microsoft.graph.responseStatus",
    "response": "String",
    "time": "String (timestamp)"
  }
}
```


---
title: "attendeeBase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# attendeeBase resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [recipient](../resources/recipient.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description** Inherited from [recipient](../resources/recipient.md)|
|type|attendeeType|**TODO: Add Description**. Possible values are: `required`, `optional`, `resource`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendeeBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendeeBase",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "String",
    "address": "String"
  },
  "type": "String"
}
```


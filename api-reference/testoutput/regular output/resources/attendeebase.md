---
title: "attendeeBase resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# attendeeBase resource type




Inherits from [recipient](../resources/recipient.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emailAddress|[emailAddress](../resources/emailAddress.md)| Inherited from [recipient](../resources/recipient.md)|
|type|Enumeration|. Possible values are: `required`, `optional`, `resource`.|

## Relationships
None

## JSON Representation
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


---
title: "attendeeBase resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# attendeeBase resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [recipient](../resources/recipient.md).

## Properties
|Property|Type|Description|
|:---|:---|:---|
|emailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description** Inherited from [recipient](../resources/recipient.md)|
|type|attendeeType|**TODO: Add Description**. Possible values are: `required`, `optional`, `resource`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.attendeeBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.attendeeBase",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "type": "String"
}
```


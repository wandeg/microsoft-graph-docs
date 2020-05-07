---
title: "InvitationV2Message resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# InvitationV2Message resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|invitationMessage|[InvitationMessage](../resources/invitationmessage.md)|**TODO: Add Description**|
|invitationTemplateID|String|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.InvitationV2Message"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.InvitationV2Message",
  "invitationTemplateID": "String",
  "invitationMessage": {
    "@odata.type": "microsoft.graph.InvitationMessage"
  }
}
```


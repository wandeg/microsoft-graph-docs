---
title: "mailTips resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mailTips resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|automaticReplies|[automaticRepliesMailTips](../resources/automaticrepliesmailtips.md)|**TODO: Add Description**|
|customMailTip|String|**TODO: Add Description**|
|deliveryRestricted|Boolean|**TODO: Add Description**|
|emailAddress|[emailAddress](../resources/emailaddress.md)|**TODO: Add Description**|
|error|[mailTipsError](../resources/mailtipserror.md)|**TODO: Add Description**|
|externalMemberCount|Int32|**TODO: Add Description**|
|isModerated|Boolean|**TODO: Add Description**|
|mailboxFull|Boolean|**TODO: Add Description**|
|maxMessageSize|Int32|**TODO: Add Description**|
|recipientScope|recipientScopeType|**TODO: Add Description**. Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonPartner`.|
|recipientSuggestions|[recipient](../resources/recipient.md) collection|**TODO: Add Description**|
|totalMemberCount|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailTips"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailTips",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress"
  },
  "automaticReplies": {
    "@odata.type": "microsoft.graph.automaticRepliesMailTips"
  },
  "mailboxFull": "Boolean",
  "customMailTip": "String",
  "externalMemberCount": "Integer",
  "totalMemberCount": "Integer",
  "deliveryRestricted": "Boolean",
  "isModerated": "Boolean",
  "recipientScope": "String",
  "recipientSuggestions": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "maxMessageSize": "Integer",
  "error": {
    "@odata.type": "microsoft.graph.mailTipsError"
  }
}
```


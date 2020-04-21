---
title: "mailTips resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
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
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mailTips"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailTips",
  "emailAddress": {
    "@odata.type": "microsoft.graph.emailAddress",
    "name": "String",
    "address": "String"
  },
  "automaticReplies": {
    "@odata.type": "microsoft.graph.automaticRepliesMailTips",
    "message": "String",
    "messageLanguage": {
      "@odata.type": "microsoft.graph.localeInfo",
      "locale": "String",
      "displayName": "String"
    },
    "scheduledStartTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone",
      "dateTime": "String",
      "timeZone": "String"
    },
    "scheduledEndTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    }
  },
  "mailboxFull": true,
  "customMailTip": "String",
  "externalMemberCount": 1024,
  "totalMemberCount": 1024,
  "deliveryRestricted": true,
  "isModerated": true,
  "recipientScope": "String",
  "recipientSuggestions": [
    {
      "@odata.type": "microsoft.graph.recipient"
    }
  ],
  "maxMessageSize": 1024,
  "error": {
    "@odata.type": "microsoft.graph.mailTipsError",
    "code": "String"
  }
}
```


---
title: "invitedUserMessageInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# invitedUserMessageInfo resource type


Namespace: Microsoft.AADInviteMgr

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|ccRecipients|[recipient](../resources/microsoft.aadinvitemgr-recipient.md) collection|**TODO: Add Description**|
|customizedMessageBody|String|**TODO: Add Description**|
|messageLanguage|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.AADInviteMgr.invitedUserMessageInfo"
}
-->
``` json
{
  "@odata.type": "#Microsoft.AADInviteMgr.invitedUserMessageInfo",
  "ccRecipients": [
    {
      "@odata.type": "Microsoft.AADInviteMgr.recipient",
      "emailAddress": {
        "@odata.type": "Microsoft.AADInviteMgr.emailAddress",
        "name": "String",
        "address": "String"
      }
    }
  ],
  "messageLanguage": "String",
  "customizedMessageBody": "String"
}
```


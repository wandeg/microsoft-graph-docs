---
title: "Get messageRule"
description: "Read properties and relationships of a messageRule object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get messageRule

Namespace: microsoft.graph

Read properties and relationships of a [messageRule](../resources/messagerule.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /invitations/{invitationsId}/invitedUser/mailFolders/{mailFolderId}/messageRules/{messageRuleId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [messageRule](../resources/messagerule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/mailFolders/{mailFolderId}/messageRules/{messageRuleId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messageRule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.messageRule",
    "id": "09801677-1677-0980-7716-800977168009",
    "displayName": "Display Name value",
    "sequence": 8,
    "conditions": {
      "@odata.type": "microsoft.graph.messageRulePredicates",
      "categories": [
        "Categories value"
      ],
      "subjectContains": [
        "Subject Contains value"
      ],
      "bodyContains": [
        "Body Contains value"
      ],
      "bodyOrSubjectContains": [
        "Body Or Subject Contains value"
      ],
      "senderContains": [
        "Sender Contains value"
      ],
      "recipientContains": [
        "Recipient Contains value"
      ],
      "headerContains": [
        "Header Contains value"
      ],
      "messageActionFlag": "String",
      "importance": "String",
      "sensitivity": "String",
      "fromAddresses": [
        {
          "@odata.type": "microsoft.graph.recipient",
          "emailAddress": {
            "@odata.type": "microsoft.graph.emailAddress",
            "name": "Name value",
            "address": "Address value"
          }
        }
      ],
      "sentToAddresses": [
        {
          "@odata.type": "microsoft.graph.recipient"
        }
      ],
      "sentToMe": true,
      "sentOnlyToMe": true,
      "sentCcMe": true,
      "sentToOrCcMe": true,
      "notSentToMe": true,
      "hasAttachments": true,
      "isApprovalRequest": true,
      "isAutomaticForward": true,
      "isAutomaticReply": true,
      "isEncrypted": true,
      "isMeetingRequest": true,
      "isMeetingResponse": true,
      "isNonDeliveryReport": true,
      "isPermissionControlled": true,
      "isReadReceipt": true,
      "isSigned": true,
      "isVoicemail": true,
      "withinSizeRange": {
        "@odata.type": "microsoft.graph.sizeRange",
        "minimumSize": 11,
        "maximumSize": 11
      }
    },
    "actions": {
      "@odata.type": "microsoft.graph.messageRuleActions",
      "moveToFolder": "Move To Folder value",
      "copyToFolder": "Copy To Folder value",
      "delete": true,
      "permanentDelete": true,
      "markAsRead": true,
      "markImportance": "String",
      "forwardTo": [
        {
          "@odata.type": "microsoft.graph.recipient"
        }
      ],
      "forwardAsAttachmentTo": [
        {
          "@odata.type": "microsoft.graph.recipient"
        }
      ],
      "redirectTo": [
        {
          "@odata.type": "microsoft.graph.recipient"
        }
      ],
      "assignCategories": [
        "Assign Categories value"
      ],
      "stopProcessingRules": true
    },
    "exceptions": {
      "@odata.type": "microsoft.graph.messageRulePredicates"
    },
    "isEnabled": true,
    "hasError": true,
    "isReadOnly": true
  }
}
```


---
title: "List messageRules"
description: "List properties and relationships of the messageRule objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List messageRules

Namespace: microsoft.graph

List properties and relationships of the [messageRule](../resources/messagerule.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/mailFolders/{mailFolderId}/messageRules
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [messageRule](../resources/messagerule.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/mailFolders/{mailFolderId}/messageRules
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.messagerule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3076

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.messageRule",
      "id": "b250e382-e382-b250-82e3-50b282e350b2",
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
  ]
}
```


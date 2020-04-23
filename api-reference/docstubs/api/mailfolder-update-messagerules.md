---
title: "Update messageRules"
description: "Update the properties of a messageRules object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update messageRules

Namespace: microsoft.graph

Update the properties of a messageRules object.

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
PATCH /invitations/{invitationsId}/invitedUser/mailFolders/{mailFolderId}/messageRules
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [messageRule](../resources/messagerule.md) object.

The following table shows the properties that are required when you create the [messageRule](../resources/messagerule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|conditions|[messageRulePredicates](../resources/messagerulepredicates.md)|**TODO: Add Description**|
|actions|[messageRuleActions](../resources/messageruleactions.md)|**TODO: Add Description**|
|exceptions|[messageRulePredicates](../resources/messagerulepredicates.md)|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|
|hasError|Boolean|**TODO: Add Description**|
|isReadOnly|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [messageRule](../resources/messagerule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_messagerules"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/mailFolders/{mailFolderId}/messageRules
Content-Type: application/json
Content-length: 2586

{
  "@odata.type": "#microsoft.graph.messageRule",
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
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.messageRule",
  "id": "78087dc2-7dc2-7808-c27d-0878c27d0878",
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
```


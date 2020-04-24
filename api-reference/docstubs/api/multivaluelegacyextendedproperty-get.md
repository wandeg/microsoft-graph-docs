---
title: "Get multiValueLegacyExtendedProperty"
description: "Read the properties and relationships of a multiValueLegacyExtendedProperty object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get multiValueLegacyExtendedProperty

Namespace: microsoft.graph

Read the properties and relationships of a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

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
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/contacts/{contactId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/event/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/mailFolders/{mailFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/contactFolders/{contactFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/event/calendar/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
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
If successful, this method returns a `200 OK` response code and a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_multivaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
    "id": "e7f135ff-35ff-e7f1-ff35-f1e7ff35f1e7",
    "value": [
      "Value value"
    ]
  }
}
```


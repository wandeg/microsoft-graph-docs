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
GET /me/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/contacts/{contactId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/messages/{messageId}/event/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/mailFolders/{mailFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/contactFolders/{contactFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/contacts/{contactId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/messages/{messageId}/event/calendar/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/messages/{messageId}/event/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/mailFolders/{mailFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/contactFolders/{contactFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/messages/{messageId}/event/calendar/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

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
GET https://graph.microsoft.com/beta/me/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
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
    "id": "3af2a6e5-a6e5-3af2-e5a6-f23ae5a6f23a",
    "value": [
      "String"
    ]
  }
}
```


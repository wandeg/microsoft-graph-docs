---
title: "Get singleValueLegacyExtendedProperty"
description: "Read the properties and relationships of a singleValueLegacyExtendedProperty object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get singleValueLegacyExtendedProperty

Namespace: microsoft.graph

Read the properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.

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
GET /me/messages/{messageId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/contacts/{contactId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/messages/{messageId}/event/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/mailFolders/{mailFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/contactFolders/{contactFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/messages/{messageId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/contacts/{contactId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/messages/{messageId}/event/calendar/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/messages/{messageId}/event/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/mailFolders/{mailFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/contactFolders/{contactFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/messages/{messageId}/event/calendar/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /groups/{groupsId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /users/{usersId}/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
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
If successful, this method returns a `200 OK` response code and a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
    "id": "351e7b94-7b94-351e-947b-1e35947b1e35",
    "value": "String"
  }
}
```


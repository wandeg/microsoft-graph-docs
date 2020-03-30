---
title: "Get singleValueLegacyExtendedProperty"
description: "Read properties and relationships of the singleValueLegacyExtendedProperty object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get singleValueLegacyExtendedProperty

Namespace: microsoft.graph

Read properties and relationships of the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

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
GET /me/messages/{messageId}/event/calendar/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "value": {
    "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
    "id": "fb40a355-a355-fb40-55a3-40fb55a340fb",
    "value": "Value value"
  }
}
```


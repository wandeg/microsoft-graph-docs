---
title: "Get multiValueLegacyExtendedProperty"
description: "Read properties and relationships of the multiValueLegacyExtendedProperty object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get multiValueLegacyExtendedProperty

Namespace: microsoft.graph

Read properties and relationships of the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

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
GET /me/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/contacts/{contactId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/messages/{messageId}/event/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/mailFolders/{mailFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/contactFolders/{contactFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/messages/{messageId}/event/calendar/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/outlook/taskGroups/{outlookTaskGroupId}/taskFolders/{outlookTaskFolderId}/tasks/{outlookTaskId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
GET /me/joinedGroups/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
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
If successful, this method returns a `200 OK` response code and [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_multivaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/messages/{messageId}/multiValueExtendedProperties/{multiValueLegacyExtendedPropertyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 191

{
  "value": {
    "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
    "id": "cafe48fc-48fc-cafe-fc48-fecafc48feca",
    "value": [
      "Value value"
    ]
  }
}
```


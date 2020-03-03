---
title: "List singleValueLegacyExtendedProperties"
description: "List properties and relationships of the singleValueLegacyExtendedProperty objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List singleValueLegacyExtendedProperties

Namespace: microsoft.graph

List properties and relationships of the [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) objects.

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
GET /me/messages/{messageId}/singleValueExtendedProperties
GET /me/contacts/{contactId}/singleValueExtendedProperties
GET /me/mailFolders/{mailFolderId}/singleValueExtendedProperties
GET /me/contactFolders/{contactFolderId}/singleValueExtendedProperties
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/singleValueExtendedProperties
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/singleValueExtendedProperties
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/singleValueExtendedProperties
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/messages/{messageId}/singleValueExtendedProperties
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.singlevaluelegacyextendedproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 196

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.singleValueLegacyExtendedProperty",
      "id": "90f9f530-f530-90f9-30f5-f99030f5f990",
      "value": "Value value"
    }
  ]
}
```


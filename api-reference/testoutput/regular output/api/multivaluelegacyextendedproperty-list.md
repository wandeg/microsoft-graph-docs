---
title: "List multiValueLegacyExtendedProperties"
description: "List properties and relationships of the multiValueLegacyExtendedProperty objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List multiValueLegacyExtendedProperties

Namespace: microsoft.graph

List properties and relationships of the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) objects.

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
GET /me/messages/{messageId}/multiValueExtendedProperties
GET /me/contacts/{contactId}/multiValueExtendedProperties
GET /me/mailFolders/{mailFolderId}/multiValueExtendedProperties
GET /me/contactFolders/{contactFolderId}/multiValueExtendedProperties
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/multiValueExtendedProperties
GET /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/multiValueExtendedProperties
GET /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/multiValueExtendedProperties
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_multivaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/messages/{messageId}/multiValueExtendedProperties
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.multivaluelegacyextendedproperty)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
      "id": "32b7bf37-bf37-32b7-37bf-b73237bfb732",
      "value": [
        "Value value"
      ]
    }
  ]
}
```


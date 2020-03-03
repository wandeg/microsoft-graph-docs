---
title: "Create multiValueLegacyExtendedProperty"
description: "Create a new multiValueLegacyExtendedProperty object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create multiValueLegacyExtendedProperty

Namespace: microsoft.graph

Create a new [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

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
POST /me/messages/{messageId}/multiValueExtendedProperties
POST /me/contacts/{contactId}/multiValueExtendedProperties
POST /me/mailFolders/{mailFolderId}/multiValueExtendedProperties
POST /me/contactFolders/{contactFolderId}/multiValueExtendedProperties
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/multiValueExtendedProperties
POST /me/messages/{messageId}/microsoft.graph.eventMessage/event/calendar/multiValueExtendedProperties
POST /me/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/multiValueExtendedProperties
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object.

The following table shows the properties that are required when you create the [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|value|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_multivaluelegacyextendedproperty_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/messages/{messageId}/multiValueExtendedProperties
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
  "value": [
    "Value value"
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.multiValueLegacyExtendedProperty",
  "id": "31b18d19-8d19-31b1-198d-b131198db131",
  "value": [
    "Value value"
  ]
}
```


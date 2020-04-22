---
title: "Get singleValueLegacyExtendedProperty"
description: "Read properties and relationships of a singleValueLegacyExtendedProperty object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get singleValueLegacyExtendedProperty

Namespace: microsoft.graph

Read properties and relationships of a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object.

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
GET /invitations/{invitationsId}/invitedUser/calendar/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/messages/{messageId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/contacts/{contactId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/calendar/events/{eventId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/mailFolders/{mailFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/contactFolders/{contactFolderId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
GET /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/conversations/{conversationId}/threads/{conversationThreadId}/posts/{postId}/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
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
If successful, this method returns a `200 OK` response code and a [singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_singlevaluelegacyextendedproperty"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/calendar/singleValueExtendedProperties/{singleValueLegacyExtendedPropertyId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
    "id": "2bf6e28c-e28c-2bf6-8ce2-f62b8ce2f62b",
    "value": "Value value"
  }
}
```


---
title: "Get teamsAppInstallation"
description: "Read properties and relationships of a teamsAppInstallation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get teamsAppInstallation

Namespace: microsoft.graph

Read properties and relationships of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.

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
GET /teams/{teamsId}/installedApps/{teamsAppInstallationId}
GET /chats/{chatsId}/installedApps/{teamsAppInstallationId}
GET /invitations/{invitationsId}/invitedUser/teamwork/installedApps/{teamsAppInstallationId}
GET /invitations/{invitationsId}/invitedUser/chats/{chatId}/installedApps/{teamsAppInstallationId}
GET /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/installedApps/{teamsAppInstallationId}
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
If successful, this method returns a `200 OK` response code and a [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_teamsappinstallation"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/installedApps/{teamsAppInstallationId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppInstallation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.teamsAppInstallation",
    "id": "76a8b1d4-b1d4-76a8-d4b1-a876d4b1a876"
  }
}
```


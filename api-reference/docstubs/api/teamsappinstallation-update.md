---
title: "Update teamsAppInstallation"
description: "Update the properties of a teamsAppInstallation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update teamsAppInstallation

Namespace: microsoft.graph

Update the properties of a [teamsAppInstallation](../resources/teamsappinstallation.md) object.

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
PATCH /teams/{teamsId}/installedApps/{teamsAppInstallationId}
PATCH /chats/{chatsId}/installedApps/{teamsAppInstallationId}
PATCH /invitations/{invitationsId}/invitedUser/teamwork/installedApps/{teamsAppInstallationId}
PATCH /invitations/{invitationsId}/invitedUser/chats/{chatId}/installedApps/{teamsAppInstallationId}
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/installedApps/{teamsAppInstallationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [teamsAppInstallation](../resources/teamsappinstallation.md) object.

The following table shows the properties that are required when you create the [teamsAppInstallation](../resources/teamsappinstallation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsAppInstallation](../resources/teamsappinstallation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_teamsappinstallation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/installedApps/{teamsAppInstallationId}
Content-Type: application/json
Content-length: 62

{
  "@odata.type": "#microsoft.graph.teamsAppInstallation"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.teamsAppInstallation",
  "id": "771c3daf-3daf-771c-af3d-1c77af3d1c77"
}
```


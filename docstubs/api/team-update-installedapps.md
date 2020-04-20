---
title: "Update installedApps"
description: "Update the properties of an installedApps object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update installedApps

Namespace: microsoft.graph

Update the properties of an installedApps object.

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
PATCH /teams/{teamsId}/installedApps
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/team/installedApps
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [teamsAppInstallation](../resources/teamsappinstallation.md) object.

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
  "name": "update_installedapps"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/installedApps
Content-Type: application/json
Content-length: 62

{
  "@odata.type": "#microsoft.graph.teamsAppInstallation"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
  "id": "6ef53a97-3a97-6ef5-973a-f56e973af56e"
}
```


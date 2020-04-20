---
title: "Create settings"
description: "Create a new settings object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create settings

Namespace: microsoft.graph

Create a new settings object.

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
POST /me/settings
POST /users/{usersId}/settings
POST /invitations/{invitationsId}/invitedUser/settings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [userSettings](../resources/usersettings.md) object.

The following table shows the properties that are required when you create the [userSettings](../resources/usersettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|contributionToContentDiscoveryDisabled|Boolean|**TODO: Add Description**|
|contributionToContentDiscoveryAsOrganizationDisabled|Boolean|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [userSettings](../resources/usersettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_usersettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/settings
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.userSettings",
  "contributionToContentDiscoveryDisabled": true,
  "contributionToContentDiscoveryAsOrganizationDisabled": true
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usersettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userSettings",
  "id": "cfb863d2-63d2-cfb8-d263-b8cfd263b8cf",
  "contributionToContentDiscoveryDisabled": true,
  "contributionToContentDiscoveryAsOrganizationDisabled": true
}
```


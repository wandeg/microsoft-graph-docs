---
title: "Update tabs"
description: "Update the properties of a tabs object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update tabs

Namespace: microsoft.graph

Update the properties of a tabs object.

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
PATCH /invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/team/channels/{channelId}/tabs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [teamsTab](../resources/teamstab.md) object.

The following table shows the properties that are required when you create the [teamsTab](../resources/teamstab.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description**|
|configuration|[teamsTabConfiguration](../resources/teamstabconfiguration.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [teamsTab](../resources/teamstab.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tabs"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/joinedTeams/{groupId}/team/channels/{channelId}/tabs
Content-Type: application/json
Content-length: 418

{
  "@odata.type": "#microsoft.graph.teamsTab",
  "displayName": "Display Name value",
  "webUrl": "https://example.com/webUrl/",
  "configuration": {
    "@odata.type": "microsoft.graph.teamsTabConfiguration",
    "entityId": "Entity Id value",
    "contentUrl": "https://example.com/contentUrl/",
    "removeUrl": "https://example.com/removeUrl/",
    "websiteUrl": "https://example.com/websiteUrl/"
  }
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
  "@odata.type": "#microsoft.graph.teamsTab",
  "id": "3b74c2ff-c2ff-3b74-ffc2-743bffc2743b",
  "displayName": "Display Name value",
  "webUrl": "https://example.com/webUrl/",
  "configuration": {
    "@odata.type": "microsoft.graph.teamsTabConfiguration",
    "entityId": "Entity Id value",
    "contentUrl": "https://example.com/contentUrl/",
    "removeUrl": "https://example.com/removeUrl/",
    "websiteUrl": "https://example.com/websiteUrl/"
  }
}
```


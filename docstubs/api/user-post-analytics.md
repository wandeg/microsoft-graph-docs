---
title: "Create analytics"
description: "Create a new analytics object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create analytics

Namespace: microsoft.graph

Create a new analytics object.

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
POST /me/analytics
POST /users/{usersId}/analytics
POST /invitations/{invitationsId}/invitedUser/analytics
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [userAnalytics](../resources/useranalytics.md) object.

The following table shows the properties that are required when you create the [userAnalytics](../resources/useranalytics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settings|[settings](../resources/settings.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [userAnalytics](../resources/useranalytics.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_useranalytics_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/analytics
Content-Type: application/json
Content-length: 206

{
  "@odata.type": "#microsoft.graph.userAnalytics",
  "settings": {
    "@odata.type": "microsoft.graph.settings",
    "hasLicense": true,
    "hasOptedOut": true,
    "hasGraphMailbox": true
  }
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.useranalytics"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userAnalytics",
  "id": "1f1ee235-e235-1f1e-35e2-1e1f35e21e1f",
  "settings": {
    "@odata.type": "microsoft.graph.settings",
    "hasLicense": true,
    "hasOptedOut": true,
    "hasGraphMailbox": true
  }
}
```


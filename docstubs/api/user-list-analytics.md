---
title: "List analytics"
description: "Get the userAnalytics from the analytics navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List analytics

Namespace: microsoft.graph

Get the userAnalytics from the analytics navigation property.

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
GET /me/analytics
GET /users/{usersId}/analytics
GET /invitations/{invitationsId}/invitedUser/analytics
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
If successful, this method returns a `200 OK` response code and a collection of [userAnalytics](../resources/useranalytics.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_useranalytics"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/analytics
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.useranalytics)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```


---
title: "Update userAnalytics"
description: "Update the properties of a userAnalytics object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userAnalytics

Namespace: microsoft.graph

Update the properties of a [userAnalytics](../resources/useranalytics.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /me/analytics
PATCH /users/{usersId}/analytics
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userAnalytics](../resources/useranalytics.md) object.

The following table shows the properties that are required when you create the [userAnalytics](../resources/useranalytics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settings|[settings](../resources/settings.md)||



## Response
If successful, this method returns a `200 OK` response code and an updated [userAnalytics](../resources/useranalytics.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_useranalytics"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/analytics
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "@odata.type": "#microsoft.graph.userAnalytics",
  "id": "1e7ff764-f764-1e7f-64f7-7f1e64f77f1e",
  "settings": {
    "@odata.type": "microsoft.graph.settings",
    "hasLicense": true,
    "hasOptedOut": true,
    "hasGraphMailbox": true
  }
}
```


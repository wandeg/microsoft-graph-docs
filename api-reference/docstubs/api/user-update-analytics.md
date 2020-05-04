---
title: "Update analytics"
description: "Update the properties of an analytics object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update analytics

Namespace: microsoft.graph

Update the properties of an analytics object.

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
PATCH /me/analytics
PATCH /users/{usersId}/analytics
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [userAnalytics](../resources/useranalytics.md) object.

The following table shows the properties that are required when you create the [userAnalytics](../resources/useranalytics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settings|[settings](../resources/settings.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [userAnalytics](../resources/useranalytics.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_analytics"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/analytics
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.userAnalytics",
  "id": "1facee1f-ee1f-1fac-1fee-ac1f1feeac1f",
  "settings": {
    "@odata.type": "microsoft.graph.settings",
    "hasLicense": true,
    "hasOptedOut": true,
    "hasGraphMailbox": true
  }
}
```


---
title: "List users"
description: "Get a list of the user objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List users

Namespace: Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models

Get a list of the [user](../resources/user.md) objects and their properties.

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
GET /user
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
If successful, this method returns a `200 OK` response code and a collection of [user](../resources/user.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_user"
}
-->
``` http
GET https://graph.microsoft.com/beta/user
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.fast.pi.viewgenerator.v2.profile.models.user)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#Microsoft.Fast.PI.ViewGenerator.V2.Profile.Models.user",
      "id": "a733a0ca-a0ca-a733-caa0-33a7caa033a7"
    }
  ]
}
```


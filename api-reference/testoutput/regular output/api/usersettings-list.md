---
title: "List userSettingses"
description: "List properties and relationships of the userSettings objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List userSettingses

Namespace: microsoft.graph

List properties and relationships of the [userSettings](../resources/usersettings.md) objects.

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
GET ** Collection URI for microsoft.graph.userSettings not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [userSettings](../resources/usersettings.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_usersettings"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.userSettings not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.usersettings)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userSettings",
      "id": "dd01d35c-d35c-dd01-5cd3-01dd5cd301dd",
      "contributionToContentDiscoveryDisabled": true,
      "contributionToContentDiscoveryAsOrganizationDisabled": true
    }
  ]
}
```


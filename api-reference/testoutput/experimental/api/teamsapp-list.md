---
title: "List teamsApps"
description: "List properties and relationships of the teamsApp objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List teamsApps

Namespace: microsoft.graph

List properties and relationships of the [teamsApp](../resources/teamsapp.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /appCatalogs/teamsApps
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [teamsApp](../resources/teamsapp.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_teamsapp"
}
-->
``` http
GET https://graph.microsoft.com/localtest/appCatalogs/teamsApps
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.teamsapp)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 294

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.teamsApp",
      "id": "64d2f22b-f22b-64d2-2bf2-d2642bf2d264",
      "externalId": "External Id value",
      "name": "Name value",
      "displayName": "Display Name value",
      "distributionMethod": "String"
    }
  ]
}
```


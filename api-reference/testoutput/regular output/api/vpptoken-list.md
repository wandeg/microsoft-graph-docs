---
title: "List vppTokens"
description: "List properties and relationships of the vppToken objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List vppTokens

Namespace: microsoft.graph

List properties and relationships of the [vppToken](../resources/vpptoken.md) objects.

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
GET /deviceAppManagement/vppTokens
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [vppToken](../resources/vpptoken.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_vpptoken"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/vppTokens
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.vpptoken)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.vppToken",
      "id": "3b31d40b-d40b-3b31-0bd4-313b0bd4313b",
      "organizationName": "Organization Name value",
      "vppTokenAccountType": "String",
      "appleId": "Apple Id value",
      "expirationDateTime": "2016-12-31T23:58:41.2128216+03:00",
      "lastSyncDateTime": "2017-01-01T00:02:54.239458+03:00",
      "token": "Token value",
      "lastModifiedDateTime": "2017-01-01T00:00:08.5199759+03:00",
      "state": "String",
      "lastSyncStatus": "String",
      "automaticallyUpdateApps": true,
      "countryOrRegion": "Country Or Region value"
    }
  ]
}
```


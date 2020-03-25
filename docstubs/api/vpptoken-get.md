---
title: "Get vppToken"
description: "Read properties and relationships of the vppToken object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get vppToken

Namespace: microsoft.graph

Read properties and relationships of the [vppToken](../resources/vpptoken.md) object.

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
GET /deviceAppManagement/vppTokens/{vppTokenId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [vppToken](../resources/vpptoken.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_vpptoken"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/vppTokens/{vppTokenId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "19ee0d84-0d84-19ee-840d-ee19840dee19",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "String",
    "appleId": "Apple Id value",
    "expirationDateTime": "2017-01-01T00:00:45.1648483+03:00",
    "lastSyncDateTime": "2016-12-31T23:56:47.3049081+03:00",
    "token": "Token value",
    "lastModifiedDateTime": "2016-12-31T23:57:04.6185814+03:00",
    "state": "String",
    "lastSyncStatus": "String",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```


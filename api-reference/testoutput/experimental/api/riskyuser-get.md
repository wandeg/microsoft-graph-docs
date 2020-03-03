---
title: "Get riskyUser"
description: "Read properties and relationships of the riskyUser object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get riskyUser

Namespace: microsoft.graph

Read properties and relationships of the [riskyUser](../resources/riskyuser.md) object.

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
GET /riskyUsers/{riskyUsersId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [riskyUser](../resources/riskyuser.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/localtest/riskyUsers/{riskyUsersId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 456

{
  "value": {
    "@odata.type": "#microsoft.graph.riskyUser",
    "id": "0f5e2830-2830-0f5e-3028-5e0f30285e0f",
    "isDeleted": true,
    "isGuest": true,
    "isProcessing": true,
    "riskLastUpdatedDateTime": "2017-01-01T00:00:07.7265805+03:00",
    "riskLevel": "String",
    "riskState": "String",
    "riskDetail": "String",
    "userDisplayName": "User Display Name value",
    "userPrincipalName": "User Principal Name value"
  }
}
```


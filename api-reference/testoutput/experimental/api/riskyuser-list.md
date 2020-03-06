---
title: "List riskyUsers"
description: "List properties and relationships of the riskyUser objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List riskyUsers

Namespace: microsoft.graph

List properties and relationships of the [riskyUser](../resources/riskyuser.md) objects.

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
GET /riskyUsers
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [riskyUser](../resources/riskyuser.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_riskyuser"
}
-->
``` http
GET https://graph.microsoft.com/localtest/riskyUsers
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyuser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 492

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUser",
      "id": "6cb2d347-d347-6cb2-47d3-b26c47d3b26c",
      "isDeleted": true,
      "isGuest": true,
      "isProcessing": true,
      "riskLastUpdatedDateTime": "2016-12-31T23:59:32.3790155+03:00",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```


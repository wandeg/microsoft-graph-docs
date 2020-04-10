---
title: "Get printUserIdentity"
description: "Read properties and relationships of the printUserIdentity object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get printUserIdentity

Namespace: microsoft.graph

Read properties and relationships of the [printUserIdentity](../resources/printuseridentity.md) object.

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
GET /print/printers/{printerId}/allowedUsers/{printUserIdentityId}
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
If successful, this method returns a `200 OK` response code and [printUserIdentity](../resources/printuseridentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printuseridentity"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}/allowedUsers/{printUserIdentityId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUserIdentity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "value": {
    "@odata.type": "#microsoft.graph.printUserIdentity",
    "id": "25f1691c-691c-25f1-1c69-f1251c69f125",
    "displayName": "Display Name value",
    "ipAddress": "Ip Address value",
    "userPrincipalName": "User Principal Name value"
  }
}
```


---
title: "List agreementAcceptances"
description: "Get the agreementAcceptances from the agreementAcceptances navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List agreementAcceptances

Namespace: microsoft.graph

Get the agreementAcceptances from the agreementAcceptances navigation property.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions. **|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/agreementAcceptances
GET /users/{usersId}/agreementAcceptances
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
If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptance"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/agreementAcceptances
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.agreementacceptance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 522

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.agreementAcceptance",
      "id": "2cb9480d-480d-2cb9-0d48-b92c0d48b92c",
      "agreementId": "Agreement Id value",
      "userId": "User Id value",
      "agreementFileId": "Agreement File Id value",
      "recordedDateTime": "2016-12-31T23:59:58.2131278+03:00",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "userEmail": "User Email value",
      "state": "String"
    }
  ]
}
```


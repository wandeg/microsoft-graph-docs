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
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /me/agreementAcceptances
GET /users/{usersId}/agreementAcceptances
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [agreementAcceptance](../resources/agreementacceptance.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_agreementacceptance"
}
-->
``` http
GET https://graph.microsoft.com/localtest/me/agreementAcceptances
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "2b6dc9c2-c9c2-2b6d-c2c9-6d2bc2c96d2b",
      "agreementId": "Agreement Id value",
      "userId": "User Id value",
      "agreementFileId": "Agreement File Id value",
      "recordedDateTime": "2016-12-31T23:56:27.4887157+03:00",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "userEmail": "User Email value",
      "state": "String"
    }
  ]
}
```


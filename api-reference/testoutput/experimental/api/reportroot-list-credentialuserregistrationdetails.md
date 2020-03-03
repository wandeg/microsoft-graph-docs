---
title: "List credentialUserRegistrationDetails"
description: "Get the credentialUserRegistrationDetailses from the credentialUserRegistrationDetails navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List credentialUserRegistrationDetails

Get the credentialUserRegistrationDetailses from the credentialUserRegistrationDetails navigation property.

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
GET /reports/credentialUserRegistrationDetails
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/docs\api/reports/credentialUserRegistrationDetails
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.credentialuserregistrationdetails)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 440

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.credentialUserRegistrationDetails",
      "id": "a1fb7134-7134-a1fb-3471-fba13471fba1",
      "userPrincipalName": "User Principal Name value",
      "userDisplayName": "User Display Name value",
      "authMethods": [
        "String"
      ],
      "isRegistered": true,
      "isEnabled": true,
      "isCapable": true,
      "isMfaRegistered": true
    }
  ]
}
```


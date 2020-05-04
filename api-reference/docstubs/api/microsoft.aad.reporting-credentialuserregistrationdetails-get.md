---
title: "Get credentialUserRegistrationDetails"
description: "Read properties and relationships of a credentialUserRegistrationDetails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get credentialUserRegistrationDetails

Namespace: Microsoft.AAD.Reporting

Read properties and relationships of a [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/credentialUserRegistrationDetails/{credentialUserRegistrationDetailsId}
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
If successful, this method returns a `200 OK` response code and a [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_credentialuserregistrationdetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails/{credentialUserRegistrationDetailsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.credentialUserRegistrationDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.credentialUserRegistrationDetails",
    "id": "bedf3cf6-3cf6-bedf-f63c-dfbef63cdfbe",
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
}
```


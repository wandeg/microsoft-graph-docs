---
title: "Update credentialUserRegistrationDetails"
description: "Update the properties of a credentialUserRegistrationDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update credentialUserRegistrationDetails

Namespace: Microsoft.AAD.Reporting

Update the properties of a [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.

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
PATCH /reports/credentialUserRegistrationDetails/{credentialUserRegistrationDetailsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.

The following table shows the properties that are required when you create the [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|userPrincipalName|String||
|userDisplayName|String||
|authMethods|Enumeration collection| Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobilePhone`, `fido`, `appPassword`, `unknownFutureValue`.|
|isRegistered|Boolean||
|isEnabled|Boolean||
|isCapable|Boolean||
|isMfaRegistered|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_credentialuserregistrationdetails"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails/{credentialUserRegistrationDetailsId}
Content-type: application/json
Content-length: 322

{
  "@odata.type": "#Microsoft.AAD.Reporting.credentialUserRegistrationDetails",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 371

{
  "@odata.type": "#Microsoft.AAD.Reporting.credentialUserRegistrationDetails",
  "id": "100598db-98db-1005-db98-0510db980510",
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
```


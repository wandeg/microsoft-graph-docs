---
title: "Add credentialUserRegistrationDetails"
description: "Add credentialUserRegistrationDetails by posting to the credentialUserRegistrationDetails collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add credentialUserRegistrationDetails

Namespace: Microsoft.AAD.Reporting

Add credentialUserRegistrationDetails by posting to the credentialUserRegistrationDetails collection.

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
POST /reports/credentialUserRegistrationDetails/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_credentialuserregistrationdetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
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
  "truncated": true,
  "@odata.type": "microsoft.aad.reporting.credentialuserregistrationdetails"
}
-->
``` http
HTTP/1.1 201 Created
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


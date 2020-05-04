---
title: "Create credentialUserRegistrationDetails"
description: "Create a new credentialUserRegistrationDetails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create credentialUserRegistrationDetails

Namespace: Microsoft.AAD.Reporting

Create a new credentialUserRegistrationDetails object.

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
POST /reports/credentialUserRegistrationDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md) object.

The following table shows the properties that are required when you create the [credentialUserRegistrationDetails](../resources/microsoft.aad.reporting-credentialuserregistrationdetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|authMethods|registrationAuthMethod collection|**TODO: Add Description**. Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobilePhone`, `fido`, `appPassword`, `unknownFutureValue`.|
|isRegistered|Boolean|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|
|isCapable|Boolean|**TODO: Add Description**|
|isMfaRegistered|Boolean|**TODO: Add Description**|



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
Content-Type: application/json
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
{
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
```


---
title: "Update credentialUserRegistrationDetails"
description: "Update the properties of a credentialUserRegistrationDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update credentialUserRegistrationDetails

Namespace: microsoft.graph

Update the properties of a [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object.

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
PATCH /reports/credentialUserRegistrationDetails/{credentialUserRegistrationDetailsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object.

The following table shows the properties that are required when you create the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String||
|userDisplayName|String||
|authMethods|Enumeration collection|. Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobilePhone`, `fido`, `appPassword`, `unknownFutureValue`.|
|isRegistered|Boolean||
|isEnabled|Boolean||
|isCapable|Boolean||
|isMfaRegistered|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_credentialuserregistrationdetails"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/reports/credentialUserRegistrationDetails/{credentialUserRegistrationDetailsId}
Content-type: application/json
Content-length: 314

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationDetails",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 363

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationDetails",
  "id": "0fd663e2-63e2-0fd6-e263-d60fe263d60f",
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


---
title: "Update credentialUserRegistrationDetails"
description: "Update the properties of a credentialUserRegistrationDetails object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update credentialUserRegistrationDetails
Namespace: microsoft.graph

Update the properties of a credentialUserRegistrationDetails object.

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
PATCH /reports/credentialUserRegistrationDetails
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object.

The following table shows the properties that are required when you create the [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|authMethods|registrationAuthMethod collection|**TODO: Add Description**. Possible values are: `email`, `mobilePhone`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobilePhone`, `fido`, `appPassword`, `unknownFutureValue`.|
|isRegistered|Boolean|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|
|isCapable|Boolean|**TODO: Add Description**|
|isMfaRegistered|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [credentialUserRegistrationDetails](../resources/credentialuserregistrationdetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_credentialuserregistrationdetails"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/credentialUserRegistrationDetails
Content-Type: application/json
Content-length: 298

{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationDetails",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "authMethods": [
    "String"
  ],
  "isRegistered": "Boolean",
  "isEnabled": "Boolean",
  "isCapable": "Boolean",
  "isMfaRegistered": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.credentialUserRegistrationDetails",
  "id": "2162c64c-c64c-2162-4cc6-62214cc66221",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "authMethods": [
    "String"
  ],
  "isRegistered": "Boolean",
  "isEnabled": "Boolean",
  "isCapable": "Boolean",
  "isMfaRegistered": "Boolean"
}
```


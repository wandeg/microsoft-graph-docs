---
title: "Update smsAuthenticationMethod"
description: "Update the properties of a smsAuthenticationMethod object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update smsAuthenticationMethod

Namespace: microsoft.graph

Update the properties of a [smsAuthenticationMethod](../resources/smsauthenticationmethod.md) object.

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
PATCH /me/authentication/smsMethods/{smsAuthenticationMethodId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [smsAuthenticationMethod](../resources/smsauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [smsAuthenticationMethod](../resources/smsauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|phoneNumber|String||
|phoneType|Enumeration| Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|
|signInState|Enumeration| Possible values are: `notSupported`, `notAllowedByPolicy`, `notProvisioned`, `phoneNumberCollision`, `provisioned`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [smsAuthenticationMethod](../resources/smsauthenticationmethod.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_smsauthenticationmethod"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/authentication/smsMethods/{smsAuthenticationMethodId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethod",
  "phoneNumber": "Phone Number value",
  "phoneType": "String",
  "signInState": "String"
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
Content-Length: 208

{
  "@odata.type": "#microsoft.graph.smsAuthenticationMethod",
  "id": "e5563d9b-3d9b-e556-9b3d-56e59b3d56e5",
  "phoneNumber": "Phone Number value",
  "phoneType": "String",
  "signInState": "String"
}
```


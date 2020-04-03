---
title: "Update phoneAuthenticationMethod"
description: "Update the properties of a phoneAuthenticationMethod object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update phoneAuthenticationMethod

Namespace: microsoft.graph

Update the properties of a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.

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
PATCH /me/authentication/phoneMethods/{phoneAuthenticationMethodId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|phoneNumber|String||
|phoneType|Enumeration| Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|
|smsSignInState|Enumeration| Possible values are: `notSupported`, `notAllowedByPolicy`, `notEnabled`, `phoneNumberNotUnique`, `ready`, `notConfigured`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_phoneauthenticationmethod"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/authentication/phoneMethods/{phoneAuthenticationMethodId}
Content-type: application/json
Content-length: 164

{
  "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "phoneNumber": "Phone Number value",
  "phoneType": "String",
  "smsSignInState": "String"
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
Content-Length: 213

{
  "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "id": "0c94a1b2-a1b2-0c94-b2a1-940cb2a1940c",
  "phoneNumber": "Phone Number value",
  "phoneType": "String",
  "smsSignInState": "String"
}
```


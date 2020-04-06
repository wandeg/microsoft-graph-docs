---
title: "Add phoneMethods"
description: "Add phoneMethods by posting to the phoneMethods collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add phoneMethods

Namespace: microsoft.graph

Add phoneMethods by posting to the phoneMethods collection.

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
POST /me/authentication/phoneMethods/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [phoneAuthenticationMethod](../resources/phoneauthenticationmethod.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_phoneauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/authentication/phoneMethods
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
  "truncated": true,
  "@odata.type": "microsoft.graph.phoneauthenticationmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 213

{
  "@odata.type": "#microsoft.graph.phoneAuthenticationMethod",
  "id": "274fa955-a955-274f-55a9-4f2755a94f27",
  "phoneNumber": "Phone Number value",
  "phoneType": "String",
  "smsSignInState": "String"
}
```


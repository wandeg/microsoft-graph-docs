---
title: "Update authenticationMethodTarget"
description: "Update the properties of a authenticationMethodTarget object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update authenticationMethodTarget

Namespace: microsoft.authMethodPolicy

Update the properties of a [authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) object.

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
PATCH /authenticationMethodConfigurations/{authenticationMethodConfigurationsId}/includeTargets/{authenticationMethodTargetId}
PATCH /authenticationMethodsPolicy/authenticationMethodConfigurations/{authenticationMethodConfigurationId}/includeTargets/{authenticationMethodTargetId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) object.

The following table shows the properties that are required when you create the [authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md).

|Property|Type|Description|
|:---|:---|:---|
|targetType|Enumeration| Possible values are: `user`, `group`, `unknownFutureValue`.|
|id|String||
|isRegistrationRequired|Boolean||
|useForSignIn|Boolean||



## Response
If successful, this method returns a `200 OK` response code and an updated [authenticationMethodTarget](../resources/microsoft.authmethodpolicy-authenticationmethodtarget.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_authenticationmethodtarget"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/authenticationMethodConfigurations/{authenticationMethodConfigurationsId}/includeTargets/{authenticationMethodTargetId}
Content-type: application/json
Content-length: 166

{
  "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodTarget",
  "targetType": "String",
  "isRegistrationRequired": true,
  "useForSignIn": true
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
Content-Length: 215

{
  "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodTarget",
  "targetType": "String",
  "id": "4ad1b251-b251-4ad1-51b2-d14a51b2d14a",
  "isRegistrationRequired": true,
  "useForSignIn": true
}
```


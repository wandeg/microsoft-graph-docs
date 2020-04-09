---
title: "Add authenticationMethodConfigurations"
description: "Add authenticationMethodConfigurations by posting to the authenticationMethodConfigurations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add authenticationMethodConfigurations

Namespace: microsoft.authMethodPolicy

Add authenticationMethodConfigurations by posting to the authenticationMethodConfigurations collection.

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
POST /authenticationMethodsPolicy/authenticationMethodConfigurations/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) object.

The following table shows the properties that are required when you create the [authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|state|Enumeration| Possible values are: `enabled`, `disabled`.|



## Response
If successful, this method returns a `201 Created` response code and a [authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_authenticationmethodconfiguration_from_authenticationmethodconfigurations"
}
-->
``` http
POST https://graph.microsoft.com/beta/authenticationMethodsPolicy/authenticationMethodConfigurations
Content-type: application/json
Content-length: 108

{
  "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodConfiguration",
  "state": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.authmethodpolicy.authenticationmethodconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 157

{
  "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodConfiguration",
  "id": "866e3a74-3a74-866e-743a-6e86743a6e86",
  "state": "String"
}
```


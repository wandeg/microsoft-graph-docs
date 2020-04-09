---
title: "Get authenticationMethodConfiguration"
description: "Read properties and relationships of the authenticationMethodConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get authenticationMethodConfiguration

Namespace: microsoft.authMethodPolicy

Read properties and relationships of the [authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) object.

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
GET /authenticationMethodConfigurations/{authenticationMethodConfigurationsId}
GET /authenticationMethodsPolicy/authenticationMethodConfigurations/{authenticationMethodConfigurationId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [authenticationMethodConfiguration](../resources/microsoft.authmethodpolicy-authenticationmethodconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_authenticationmethodconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/authenticationMethodConfigurations/{authenticationMethodConfigurationsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.authMethodPolicy.authenticationMethodConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "value": {
    "@odata.type": "#microsoft.authMethodPolicy.authenticationMethodConfiguration",
    "id": "866e3a74-3a74-866e-743a-6e86743a6e86",
    "state": "String"
  }
}
```


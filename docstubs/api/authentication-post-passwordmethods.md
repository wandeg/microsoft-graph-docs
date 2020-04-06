---
title: "Add passwordMethods"
description: "Add passwordMethods by posting to the passwordMethods collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add passwordMethods

Namespace: microsoft.graph

Add passwordMethods by posting to the passwordMethods collection.

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
POST /me/authentication/passwordMethods/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|password|String||
|creationDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [passwordAuthenticationMethod](../resources/passwordauthenticationmethod.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_passwordauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/authentication/passwordMethods
Content-type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
  "password": "Password value",
  "creationDateTime": "2017-01-01T00:02:15.7719196+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.passwordauthenticationmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.passwordAuthenticationMethod",
  "id": "2cec7555-7555-2cec-5575-ec2c5575ec2c",
  "password": "Password value",
  "creationDateTime": "2017-01-01T00:02:15.7719196+00:00"
}
```


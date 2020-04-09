---
title: "Update voiceAuthenticationMethod"
description: "Update the properties of a voiceAuthenticationMethod object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update voiceAuthenticationMethod

Namespace: microsoft.graph

Update the properties of a [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) object.

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
PATCH /me/authentication/voiceMethods/{voiceAuthenticationMethodId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|phoneNumber|String||
|phoneType|Enumeration| Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_voiceauthenticationmethod"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/authentication/voiceMethods/{voiceAuthenticationMethodId}
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.voiceAuthenticationMethod",
  "phoneNumber": "Phone Number value",
  "phoneType": "String"
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
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.voiceAuthenticationMethod",
  "id": "b5139fd0-9fd0-b513-d09f-13b5d09f13b5",
  "phoneNumber": "Phone Number value",
  "phoneType": "String"
}
```


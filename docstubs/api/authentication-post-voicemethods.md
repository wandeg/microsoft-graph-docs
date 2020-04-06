---
title: "Add voiceMethods"
description: "Add voiceMethods by posting to the voiceMethods collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add voiceMethods

Namespace: microsoft.graph

Add voiceMethods by posting to the voiceMethods collection.

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
POST /me/authentication/voiceMethods/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) object.

The following table shows the properties that are required when you create the [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|phoneNumber|String||
|phoneType|Enumeration| Possible values are: `mobile`, `alternateMobile`, `office`, `unknownFutureValue`.|



## Response
If successful, this method returns a `201 Created` response code and a [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_voiceauthenticationmethod_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/authentication/voiceMethods
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
  "truncated": true,
  "@odata.type": "microsoft.graph.voiceauthenticationmethod"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.voiceAuthenticationMethod",
  "id": "ef93ad85-ad85-ef93-85ad-93ef85ad93ef",
  "phoneNumber": "Phone Number value",
  "phoneType": "String"
}
```


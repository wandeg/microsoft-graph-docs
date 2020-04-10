---
title: "List voiceMethods"
description: "Get the voiceAuthenticationMethods from the voiceMethods navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List voiceMethods

Namespace: microsoft.graph

Get the voiceAuthenticationMethods from the voiceMethods navigation property.

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
GET /me/authentication/voiceMethods
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
If successful, this method returns a `200 OK` response code and a collection of [voiceAuthenticationMethod](../resources/voiceauthenticationmethod.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_voiceauthenticationmethod"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/authentication/voiceMethods
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.voiceauthenticationmethod)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 231

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.voiceAuthenticationMethod",
      "id": "9920f9ae-f9ae-9920-aef9-2099aef92099",
      "phoneNumber": "Phone Number value",
      "phoneType": "String"
    }
  ]
}
```


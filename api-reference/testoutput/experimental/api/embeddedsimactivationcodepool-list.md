---
title: "List embeddedSIMActivationCodePools"
description: "List properties and relationships of the embeddedSIMActivationCodePool objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List embeddedSIMActivationCodePools

Namespace: microsoft.graph

List properties and relationships of the [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/embeddedSIMActivationCodePools
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [embeddedSIMActivationCodePool](../resources/embeddedsimactivationcodepool.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_embeddedsimactivationcodepool"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/embeddedSIMActivationCodePools
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.embeddedsimactivationcodepool)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 716

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
      "id": "c32a6b75-6b75-c32a-756b-2ac3756b2ac3",
      "displayName": "Display Name value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00",
      "activationCodes": [
        {
          "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
          "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
          "matchingIdentifier": "Matching Identifier value",
          "smdpPlusServerAddress": "Smdp Plus Server Address value"
        }
      ],
      "activationCodeCount": 3
    }
  ]
}
```


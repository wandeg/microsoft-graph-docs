---
title: "Get trustFrameworkKeySet"
description: "Read properties and relationships of the trustFrameworkKeySet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get trustFrameworkKeySet

Namespace: microsoft.graph

Read properties and relationships of the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.

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
GET /trustFramework/keySets/{trustFrameworkKeySetId}
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
If successful, this method returns a `200 OK` response code and [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}
-->
``` http
GET https://graph.microsoft.com/beta/trustFramework/keySets/{trustFrameworkKeySetId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKeySet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 673

{
  "value": {
    "@odata.type": "#microsoft.graph.trustFrameworkKeySet",
    "id": "9f787ee0-7ee0-9f78-e07e-789fe07e789f",
    "keys": [
      {
        "@odata.type": "microsoft.graph.trustFrameworkKey",
        "k": "K value",
        "x5c": [
          "X5c value"
        ],
        "x5t": "X5t value",
        "kty": "Kty value",
        "use": "Use value",
        "exp": 3,
        "nbf": 3,
        "kid": "Kid value",
        "e": "E value",
        "n": "N value",
        "d": "D value",
        "p": "P value",
        "q": "Q value",
        "dp": "Dp value",
        "dq": "Dq value",
        "qi": "Qi value"
      }
    ]
  }
}
```


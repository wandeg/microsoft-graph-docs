---
title: "Update trustFrameworkKeySet"
description: "Update the properties of a trustFrameworkKeySet object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update trustFrameworkKeySet

Namespace: microsoft.graph

Update the properties of a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.

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
PATCH /trustFramework/keySets/{trustFrameworkKeySetId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.

The following table shows the properties that are required when you create the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|keys|[trustFrameworkKey](../resources/trustframeworkkey.md) collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_trustframeworkkeyset"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/trustFramework/keySets/{trustFrameworkKeySetId}
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.trustFrameworkKeySet",
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
Content-Length: 604

{
  "@odata.type": "#microsoft.graph.trustFrameworkKeySet",
  "id": "f061e7f8-e7f8-f061-f8e7-61f0f8e761f0",
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
```


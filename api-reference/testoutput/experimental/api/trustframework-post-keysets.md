---
title: "Add keySets"
description: "Add keySets by posting to the keySets collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add keySets

Namespace: microsoft.graph

Add keySets by posting to the keySets collection.

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
POST /trustFramework/keySets/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.

The following table shows the properties that are required when you create the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|keys|[trustFrameworkKey](../resources/trustframeworkkey.md) collection||



## Response
If successful, this method returns a `201 Created` response code and a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/trustFramework/keySets
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
  "truncated": true,
  "@odata.type": "microsoft.graph.trustframeworkkeyset"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 604

{
  "@odata.type": "#microsoft.graph.trustFrameworkKeySet",
  "id": "c5e99ec4-9ec4-c5e9-c49e-e9c5c49ee9c5",
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


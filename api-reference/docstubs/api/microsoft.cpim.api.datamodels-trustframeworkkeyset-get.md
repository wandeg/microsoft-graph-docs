---
title: "Get trustFrameworkKeySet"
description: "Read properties and relationships of a trustFrameworkKeySet object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get trustFrameworkKeySet

Namespace: microsoft.cpim.api.dataModels

Read properties and relationships of a [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

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
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_trustframeworkkeyset"
}
-->
``` http
GET https://graph.microsoft.com/beta/trustFramework/keySets/{trustFrameworkKeySetId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.dataModels.trustFrameworkKeySet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.cpim.api.dataModels.trustFrameworkKeySet",
    "id": "dfa19ec0-9ec0-dfa1-c09e-a1dfc09ea1df",
    "keys": [
      {
        "@odata.type": "microsoft.cpim.api.dataModels.trustFrameworkKey",
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


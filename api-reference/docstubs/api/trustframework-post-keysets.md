---
title: "Create keySets"
description: "Create a new keySets object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create keySets

Namespace: microsoft.graph

Create a new keySets object.

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
POST /trustFramework/keySets
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object.

The following table shows the properties that are required when you create the [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|keys|[trustFrameworkKey](../resources/trustframeworkkey.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_trustframeworkkeyset_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/trustFramework/keySets
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustframeworkkeyset"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.trustFrameworkKeySet",
  "id": "0c33c5cd-c5cd-0c33-cdc5-330ccdc5330c",
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


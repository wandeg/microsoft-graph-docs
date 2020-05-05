---
title: "Create keySets"
description: "Create a new keySets object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create keySets

Namespace: microsoft.cpim.api.dataModels

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
In the request body, supply a JSON representation for the [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) object.

The following table shows the properties that are required when you create the [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|keys|[trustFrameworkKey](../resources/microsoft.cpim.api.datamodels-trustframeworkkey.md) collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [trustFrameworkKeySet](../resources/microsoft.cpim.api.datamodels-trustframeworkkeyset.md) object in the response body.

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
Content-length: 583

{
  "@odata.type": "#microsoft.cpim.api.dataModels.trustFrameworkKeySet",
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
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.cpim.api.datamodels.trustframeworkkeyset"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
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
```


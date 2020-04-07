---
title: "generateKey"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# generateKey

Namespace: microsoft.graph



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
POST /trustFramework/keySets/{trustFrameworkKeySetId}/generateKey
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Property|Type|Description|
|:---|:---|:---|
|use|String||
|kty|String||
|nbf|Int64||
|exp|Int64||



## Response
If successful, this action returns a `200 OK` response code and a [trustFrameworkKey](../resources/trustframeworkkey.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_generatekey"
}
-->
``` http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{trustFrameworkKeySetId}/generateKey

Content-type: application/json
Content-length: 75

{
  "use": "Use value",
  "kty": "Kty value",
  "nbf": 3,
  "exp": 3
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustframeworkkey"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": {
    "@odata.type": "microsoft.graph.trustFrameworkKey"
  }
}
```


---
title: "getActiveKey"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getActiveKey

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
GET /trustFramework/keySets/{trustFrameworkKeySetId}/getActiveKey
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this function returns a `200 OK` response code and a [trustFrameworkKey](../resources/trustframeworkkey.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}
-->
``` http
GET https://graph.microsoft.com/beta/trustFramework/keySets/{trustFrameworkKeySetId}/getActiveKey
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


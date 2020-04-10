---
title: "tiIndicator: deleteTiIndicators"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# deleteTiIndicators

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
POST /Security/tiIndicators/deleteTiIndicators
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
|value|String collection||



## Response
If successful, this action returns a `200 OK` response code and a [ResultInfo](../resources/resultinfo.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "tiindicator_deletetiindicators"
}
-->
``` http
POST https://graph.microsoft.com/beta/Security/tiIndicators/deleteTiIndicators

Content-type: application/json
Content-length: 42

{
  "value": [
    "Value value"
  ]
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.resultinfo)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 88

{
  "value": [
    {
      "@odata.type": "microsoft.graph.ResultInfo"
    }
  ]
}
```


---
title: "List programControlTypes"
description: "List properties and relationships of the programControlType objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List programControlTypes

Namespace: microsoft.graph

List properties and relationships of the [programControlType](../resources/programcontroltype.md) objects.

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
GET /programControlTypes
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
If successful, this method returns a `200 OK` response code and a collection of [programControlType](../resources/programcontroltype.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_programcontroltype"
}
-->
``` http
GET https://graph.microsoft.com/beta/programControlTypes
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.programcontroltype)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 254

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.programControlType",
      "id": "193072d9-72d9-1930-d972-3019d9723019",
      "controlTypeGroupId": "Control Type Group Id value",
      "displayName": "Display Name value"
    }
  ]
}
```


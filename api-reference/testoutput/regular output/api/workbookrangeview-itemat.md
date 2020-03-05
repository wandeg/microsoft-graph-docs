---
title: "itemAt"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# itemAt

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
GET ** Collection URI for microsoft.graph.workbookRangeView not found/itemAt
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|index|Int32||



## Response
If successful, this function returns a `200 OK` response code and a [workbookRangeView](../resources/workbookrangeview.md) in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "workbookrangeview_itemat"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRangeView not found/itemAt(index=5)
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrangeview"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 782

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookRangeView",
    "id": "77bd3e84-3e84-77bd-843e-bd77843ebd77",
    "cellAddresses": {
      "@odata.type": "microsoft.graph.Json"
    },
    "columnCount": 11,
    "formulas": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasLocal": {
      "@odata.type": "microsoft.graph.Json"
    },
    "formulasR1C1": {
      "@odata.type": "microsoft.graph.Json"
    },
    "index": 5,
    "numberFormat": {
      "@odata.type": "microsoft.graph.Json"
    },
    "rowCount": 8,
    "text": {
      "@odata.type": "microsoft.graph.Json"
    },
    "valueTypes": {
      "@odata.type": "microsoft.graph.Json"
    },
    "values": {
      "@odata.type": "microsoft.graph.Json"
    }
  }
}
```


---
title: "Get workbookRangeFill"
description: "Read properties and relationships of the workbookRangeFill object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get workbookRangeFill

Namespace: microsoft.graph

Read properties and relationships of the [workbookRangeFill](../resources/workbookrangefill.md) object.

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
GET ** Entity URI for microsoft.graph.workbookRangeFill not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_workbookrangefill"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.workbookRangeFill not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRangeFill"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 160

{
  "value": {
    "@odata.type": "#microsoft.graph.workbookRangeFill",
    "id": "7c7e088b-088b-7c7e-8b08-7e7c8b087e7c",
    "color": "Color value"
  }
}
```


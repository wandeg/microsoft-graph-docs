---
title: "Update workbookRangeFill"
description: "Update the properties of a workbookRangeFill object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookRangeFill

Namespace: microsoft.graph

Update the properties of a [workbookRangeFill](../resources/workbookrangefill.md) object.

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
PATCH ** Entity URI for microsoft.graph.workbookRangeFill not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookRangeFill](../resources/workbookrangefill.md) object.

The following table shows the properties that are required when you create the [workbookRangeFill](../resources/workbookrangefill.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|color|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookrangefill"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.workbookRangeFill not found
Content-type: application/json
Content-length: 86

{
  "@odata.type": "#microsoft.graph.workbookRangeFill",
  "color": "Color value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 135

{
  "@odata.type": "#microsoft.graph.workbookRangeFill",
  "id": "7c7e088b-088b-7c7e-8b08-7e7c8b087e7c",
  "color": "Color value"
}
```


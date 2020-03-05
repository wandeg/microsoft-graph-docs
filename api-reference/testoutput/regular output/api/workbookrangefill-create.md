---
title: "Create workbookRangeFill"
description: "Create a new workbookRangeFill object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create workbookRangeFill

Namespace: microsoft.graph

Create a new [workbookRangeFill](../resources/workbookrangefill.md) object.

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
POST ** Collection URI for microsoft.graph.workbookRangeFill not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [workbookRangeFill](../resources/workbookrangefill.md) object.

The following table shows the properties that are required when you create the [workbookRangeFill](../resources/workbookrangefill.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|color|String||



## Response
If successful, this method returns a `201 Created` response code and a [workbookRangeFill](../resources/workbookrangefill.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_workbookrangefill_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.workbookRangeFill not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookrangefill"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 135

{
  "@odata.type": "#microsoft.graph.workbookRangeFill",
  "id": "7c7e088b-088b-7c7e-8b08-7e7c8b087e7c",
  "color": "Color value"
}
```


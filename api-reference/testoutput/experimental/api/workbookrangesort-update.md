---
title: "Update workbookRangeSort"
description: "Update the properties of a workbookRangeSort object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update workbookRangeSort

Namespace: microsoft.graph

Update the properties of a [workbookRangeSort](../resources/workbookrangesort.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.graph.workbookRangeSort not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [workbookRangeSort](../resources/workbookrangesort.md) object.

The following table shows the properties that are required when you create the [workbookRangeSort](../resources/workbookrangesort.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [workbookRangeSort](../resources/workbookrangesort.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_workbookrangesort"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.workbookRangeSort not found
Content-type: application/json
Content-length: 59

{
  "@odata.type": "#microsoft.graph.workbookRangeSort"
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
Content-Length: 108

{
  "@odata.type": "#microsoft.graph.workbookRangeSort",
  "id": "e613ec6c-ec6c-e613-6cec-13e66cec13e6"
}
```


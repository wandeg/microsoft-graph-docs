---
title: "Update fileClassificationRequest"
description: "Update the properties of a fileClassificationRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update fileClassificationRequest

Namespace: microsoft.graph

Update the properties of a [fileClassificationRequest](../resources/fileclassificationrequest.md) object.

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
PATCH /dataClassification/classifyFile/{fileClassificationRequestId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [fileClassificationRequest](../resources/fileclassificationrequest.md) object.

The following table shows the properties that are required when you create the [fileClassificationRequest](../resources/fileclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|file|Stream||
|sensitiveTypeIds|String collection||



## Response
If successful, this method returns a `200 OK` response code and an updated [fileClassificationRequest](../resources/fileclassificationrequest.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_fileclassificationrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/dataClassification/classifyFile/{fileClassificationRequestId}
Content-type: application/json
Content-length: 151

{
  "@odata.type": "#microsoft.graph.fileClassificationRequest",
  "file": "Stream",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ]
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
Content-Length: 200

{
  "@odata.type": "#microsoft.graph.fileClassificationRequest",
  "id": "25fefee6-fee6-25fe-e6fe-fe25e6fefe25",
  "file": "Stream",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ]
}
```


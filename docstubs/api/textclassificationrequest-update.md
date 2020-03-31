---
title: "Update textClassificationRequest"
description: "Update the properties of a textClassificationRequest object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update textClassificationRequest

Namespace: microsoft.graph

Update the properties of a [textClassificationRequest](../resources/textclassificationrequest.md) object.

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
PATCH /dataClassification/classifyText/{textClassificationRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [textClassificationRequest](../resources/textclassificationrequest.md) object.

The following table shows the properties that are required when you create the [textClassificationRequest](../resources/textclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|text|String||
|sensitiveTypeIds|String collection||
|scopesToRun|Enumeration| Possible values are: `fullDocument`, `partialDocument`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [textClassificationRequest](../resources/textclassificationrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_textclassificationrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/classifyText/{textClassificationRequestId}
Content-type: application/json
Content-length: 183

{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "text": "Text value",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ],
  "scopesToRun": "String"
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
Content-Length: 232

{
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "id": "d3c5af93-af93-d3c5-93af-c5d393afc5d3",
  "text": "Text value",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ],
  "scopesToRun": "String"
}
```


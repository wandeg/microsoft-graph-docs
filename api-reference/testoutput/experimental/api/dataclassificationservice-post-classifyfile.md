---
title: "Add classifyFile"
description: "Add classifyFile by posting to the classifyFile collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add classifyFile

Namespace: microsoft.graph

Add classifyFile by posting to the classifyFile collection.

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
POST /dataClassification/classifyFile/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [fileClassificationRequest](../resources/fileclassificationrequest.md) object.

The following table shows the properties that are required when you create the [fileClassificationRequest](../resources/fileclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|file|Stream||
|sensitiveTypeIds|String collection||



## Response
If successful, this method returns a `201 Created` response code and a [fileClassificationRequest](../resources/fileclassificationrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_fileclassificationrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/dataClassification/classifyFile
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
  "truncated": true,
  "@odata.type": "microsoft.graph.fileclassificationrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 200

{
  "@odata.type": "#microsoft.graph.fileClassificationRequest",
  "id": "456093db-93db-4560-db93-6045db936045",
  "file": "Stream",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ]
}
```


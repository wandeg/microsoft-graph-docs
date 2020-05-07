---
title: "Update classifyFile"
description: "Update the properties of a classifyFile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update classifyFile

Namespace: microsoft.graph

Update the properties of a classifyFile object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /dataClassification/classifyFile
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [fileClassificationRequest](../resources/fileclassificationrequest.md) object.

The following table shows the properties that are required when you create the [fileClassificationRequest](../resources/fileclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|file|Stream|**TODO: Add Description**|
|sensitiveTypeIds|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [fileClassificationRequest](../resources/fileclassificationrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_classifyfile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/classifyFile
Content-Type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.fileClassificationRequest",
  "file": "Stream",
  "sensitiveTypeIds": [
    "String"
  ]
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.fileClassificationRequest",
  "id": "3fb9d5ce-d5ce-3fb9-ced5-b93fced5b93f",
  "file": "Stream",
  "sensitiveTypeIds": [
    "String"
  ]
}
```


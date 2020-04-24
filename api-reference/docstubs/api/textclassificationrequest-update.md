---
title: "Update textClassificationRequest"
description: "Update the properties of a textClassificationRequest object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update textClassificationRequest

Namespace: microsoft.graph

Update the properties of a [textClassificationRequest](../resources/textclassificationrequest.md) object.

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
PATCH /dataClassification/classifyText/{textClassificationRequestId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [textClassificationRequest](../resources/textclassificationrequest.md) object.

The following table shows the properties that are required when you create the [textClassificationRequest](../resources/textclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|text|String|**TODO: Add Description**|
|sensitiveTypeIds|String collection|**TODO: Add Description**|
|scopesToRun|sensitiveTypeScope|**TODO: Add Description**. Possible values are: `fullDocument`, `partialDocument`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [textClassificationRequest](../resources/textclassificationrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_textclassificationrequest"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/classifyText/{textClassificationRequestId}
Content-Type: application/json
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
  "@odata.type": "#microsoft.graph.textClassificationRequest",
  "id": "8df80a4c-0a4c-8df8-4c0a-f88d4c0af88d",
  "text": "Text value",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ],
  "scopesToRun": "String"
}
```


---
title: "Create classifyText"
description: "Create a new classifyText object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create classifyText

Namespace: microsoft.graph

Create a new classifyText object.

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
POST /dataClassification/classifyText
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
If successful, this method returns a `201 Created` response code and a [textClassificationRequest](../resources/textclassificationrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_textclassificationrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/classifyText
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
  "truncated": true,
  "@odata.type": "microsoft.graph.textclassificationrequest"
}
-->
``` http
HTTP/1.1 201 Created
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


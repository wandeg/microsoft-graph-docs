---
title: "Create classifyFile"
description: "Create a new classifyFile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create classifyFile

Namespace: microsoft.graph

Create a new classifyFile object.

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
POST /dataClassification/classifyFile
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [fileClassificationRequest](../resources/fileclassificationrequest.md) object.

The following table shows the properties that are required when you create the [fileClassificationRequest](../resources/fileclassificationrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|file|Stream|**TODO: Add Description**|
|sensitiveTypeIds|String collection|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [fileClassificationRequest](../resources/fileclassificationrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_fileclassificationrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataClassification/classifyFile
Content-Type: application/json
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.fileclassificationrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.fileClassificationRequest",
  "id": "924bdd12-dd12-924b-12dd-4b9212dd4b92",
  "file": "Stream",
  "sensitiveTypeIds": [
    "Sensitive Type Ids value"
  ]
}
```


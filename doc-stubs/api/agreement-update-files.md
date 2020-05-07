---
title: "Update files"
description: "Update the properties of a files object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update files

Namespace: microsoft.graph

Update the properties of a files object.

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
PATCH /agreements/{agreementsId}/files
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [agreementFile](../resources/agreementfile.md) object.

The following table shows the properties that are required when you create the [agreementFile](../resources/agreementfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|language|String|**TODO: Add Description**|
|fileName|String|**TODO: Add Description**|
|fileData|[agreementFileData](../resources/agreementfiledata.md)|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [agreementFile](../resources/agreementfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_files"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/agreements/{agreementsId}/files
Content-Type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.agreementFile",
  "language": "String",
  "fileName": "String",
  "fileData": {
    "@odata.type": "microsoft.graph.agreementFileData"
  },
  "isDefault": "Boolean"
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
  "@odata.type": "#microsoft.graph.agreementFile",
  "id": "ffa6c14e-c14e-ffa6-4ec1-a6ff4ec1a6ff",
  "language": "String",
  "fileName": "String",
  "fileData": {
    "@odata.type": "microsoft.graph.agreementFileData"
  },
  "isDefault": "Boolean"
}
```


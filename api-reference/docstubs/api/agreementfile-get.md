---
title: "Get agreementFile"
description: "Read the properties and relationships of an agreementFile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get agreementFile

Namespace: microsoft.graph

Read the properties and relationships of an [agreementFile](../resources/agreementfile.md) object.

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
GET /agreements/{agreementsId}/files/{agreementFileId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and an [agreementFile](../resources/agreementfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_agreementfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/agreements/{agreementsId}/files/{agreementFileId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreementFile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.agreementFile",
    "id": "fe0d8075-8075-fe0d-7580-0dfe75800dfe",
    "language": "Language value",
    "fileName": "File Name value",
    "fileData": {
      "@odata.type": "microsoft.graph.agreementFileData",
      "data": "ZGF0YQ=="
    },
    "isDefault": true
  }
}
```


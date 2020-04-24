---
title: "Get dataPolicyOperation"
description: "Read the properties and relationships of a dataPolicyOperation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get dataPolicyOperation

Namespace: microsoft.graph

Read the properties and relationships of a [dataPolicyOperation](../resources/datapolicyoperation.md) object.

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
GET /dataPolicyOperations/{dataPolicyOperationsId}
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
If successful, this method returns a `200 OK` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_datapolicyoperation"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataPolicyOperations/{dataPolicyOperationsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.dataPolicyOperation"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.dataPolicyOperation",
    "id": "ba170cba-0cba-ba17-ba0c-17baba0c17ba",
    "completedDateTime": "2017-01-01T00:02:03.9770517+03:00",
    "status": "String",
    "storageLocation": "Storage Location value",
    "userId": "User Id value",
    "submittedDateTime": "2017-01-01T00:03:16.4748996+03:00",
    "progress": "Double"
  }
}
```


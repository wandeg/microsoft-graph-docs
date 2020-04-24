---
title: "Get contract"
description: "Read the properties and relationships of a contract object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get contract

Namespace: microsoft.graph

Read the properties and relationships of a [contract](../resources/contract.md) object.

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
GET /contracts/{contractsId}
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
If successful, this method returns a `200 OK` response code and a [contract](../resources/contract.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_contract"
}
-->
``` http
GET https://graph.microsoft.com/beta/contracts/{contractsId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.contract",
    "id": "f5a78caf-8caf-f5a7-af8c-a7f5af8ca7f5",
    "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
    "contractType": "Contract Type value",
    "customerId": "c235ff35-ff35-c235-35ff-35c235ff35c2",
    "defaultDomainName": "Default Domain Name value",
    "displayName": "Display Name value"
  }
}
```


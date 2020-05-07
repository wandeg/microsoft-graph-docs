---
title: "Get sensitiveType"
description: "Read the properties and relationships of a sensitiveType object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get sensitiveType

Namespace: microsoft.graph

Read the properties and relationships of a [sensitiveType](../resources/sensitivetype.md) object.

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
GET /dataClassification/sensitiveTypes/{sensitiveTypeId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [sensitiveType](../resources/sensitivetype.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sensitivetype"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/sensitiveTypes/{sensitiveTypeId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitiveType"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.sensitiveType",
    "id": "fd7ea928-a928-fd7e-28a9-7efd28a97efd",
    "name": "String",
    "description": "String",
    "rulePackageId": "String",
    "rulePackageType": "String",
    "publisherName": "String",
    "state": "String",
    "scope": "String"
  }
}
```


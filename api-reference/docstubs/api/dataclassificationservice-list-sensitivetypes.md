---
title: "List sensitiveTypes"
description: "Get the sensitiveTypes from the sensitiveTypes navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List sensitiveTypes

Namespace: microsoft.graph

Get the sensitiveTypes from the sensitiveTypes navigation property.

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
GET /dataClassification/sensitiveTypes
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
If successful, this method returns a `200 OK` response code and a collection of [sensitiveType](../resources/sensitivetype.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sensitivetype"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/sensitiveTypes
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sensitivetype)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sensitiveType",
      "id": "1fdf7c8f-7c8f-1fdf-8f7c-df1f8f7cdf1f",
      "name": "Name value",
      "description": "Description value",
      "rulePackageId": "Rule Package Id value",
      "rulePackageType": "Rule Package Type value",
      "publisherName": "Publisher Name value",
      "state": "State value",
      "scope": "String"
    }
  ]
}
```


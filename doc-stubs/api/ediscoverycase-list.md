---
title: "List ediscoveryCases"
description: "Get a list of the ediscoveryCase objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List ediscoveryCases
Namespace: microsoft.graph

Get a list of the [ediscoveryCase](../resources/ediscoverycase.md) objects and their properties.

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
GET /compliance/ediscovery/cases
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

If successful, this method returns a `200 OK` response code and a collection of [ediscoveryCase](../resources/ediscoverycase.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycase"
}
-->
``` http
GET https://graph.microsoft.com/beta/compliance/ediscovery/cases
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.ediscoverycase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscoveryCase",
      "id": "e7a6b4cf-b4cf-e7a6-cfb4-a6e7cfb4a6e7",
      "description": "String",
      "createdBy": "String",
      "lastModifiedBy": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "status": "String",
      "closedBy": "String",
      "closedDateTime": "String (timestamp)",
      "externalId": "String",
      "displayName": "String",
      "createdDateTime": "String (timestamp)"
    }
  ]
}
```


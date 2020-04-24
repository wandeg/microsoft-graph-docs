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
GET /cases
GET /compliance/ediscovery/cases
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
If successful, this method returns a `200 OK` response code and a collection of [ediscoveryCase](../resources/ediscoverycase.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycase"
}
-->
``` http
GET https://graph.microsoft.com/beta/cases
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
      "id": "e2727eb4-7eb4-e272-b47e-72e2b47e72e2",
      "description": "Description value",
      "createdBy": "Created By value",
      "lastModifiedBy": "Last Modified By value",
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
      "status": "String",
      "closedBy": "Closed By value",
      "closedDateTime": "2016-12-31T23:58:06.1799456+03:00",
      "externalId": "External Id value",
      "displayName": "Display Name value",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00"
    }
  ]
}
```


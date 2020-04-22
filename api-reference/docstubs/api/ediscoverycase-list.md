---
title: "List ediscoveryCases"
description: "Get a list of the ediscoveryCase objects and their properties."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
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
      "id": "2a8e316b-316b-2a8e-6b31-8e2a6b318e2a",
      "description": "Description value",
      "createdBy": "Created By value",
      "lastModifiedBy": "Last Modified By value",
      "lastModifiedDateTime": "2017-01-01T00:00:09.5385853+00:00",
      "status": "String",
      "closedBy": "Closed By value",
      "closedDateTime": "2016-12-31T23:57:03.2743031+00:00",
      "externalId": "External Id value",
      "displayName": "Display Name value",
      "createdDateTime": "2016-12-31T23:57:19.8403601+00:00"
    }
  ]
}
```


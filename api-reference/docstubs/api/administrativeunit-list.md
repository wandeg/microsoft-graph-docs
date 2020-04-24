---
title: "List administrativeUnits"
description: "Get a list of the administrativeUnit objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List administrativeUnits

Namespace: microsoft.graph

Get a list of the [administrativeUnit](../resources/administrativeunit.md) objects and their properties.

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
GET /administrativeUnits
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
If successful, this method returns a `200 OK` response code and a collection of [administrativeUnit](../resources/administrativeunit.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_administrativeunit"
}
-->
``` http
GET https://graph.microsoft.com/beta/administrativeUnits
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.administrativeunit)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.administrativeUnit",
      "id": "64381005-1005-6438-0510-386405103864",
      "deletedDateTime": "2017-01-01T00:02:07.4980046+03:00",
      "displayName": "Display Name value",
      "description": "Description value",
      "visibility": "Visibility value"
    }
  ]
}
```


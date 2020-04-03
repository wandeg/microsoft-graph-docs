---
title: "Get taxGroup"
description: "Read properties and relationships of the taxGroup object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get taxGroup

Namespace: microsoft.graph

Read properties and relationships of the [taxGroup](../resources/taxgroup.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/taxGroups/{taxGroupId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [taxGroup](../resources/taxgroup.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_taxgroup"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/taxGroups/{taxGroupId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.taxGroup"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.taxGroup",
    "id": "3b13dede-dede-3b13-dede-133bdede133b",
    "code": "Code value",
    "displayName": "Display Name value",
    "taxType": "Tax Type value",
    "lastModifiedDateTime": "2017-01-01T00:02:04.9650039+00:00"
  }
}
```


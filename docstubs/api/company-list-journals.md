---
title: "List journals"
description: "Get the journals from the journals navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List journals

Namespace: microsoft.graph

Get the journals from the journals navigation property.

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
GET /financials/companies/{companyId}/journals
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
If successful, this method returns a `200 OK` response code and a collection of [journal](../resources/journal.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_journal"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/journals
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.journal)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 416

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.journal",
      "id": "06bfc720-c720-06bf-20c7-bf0620c7bf06",
      "code": "Code value",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00",
      "balancingAccountId": "6cdf2014-2014-6cdf-1420-df6c1420df6c",
      "balancingAccountNumber": "Balancing Account Number value"
    }
  ]
}
```


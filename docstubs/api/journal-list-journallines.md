---
title: "List journalLines"
description: "Get the journalLines from the journalLines navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List journalLines

Namespace: microsoft.graph

Get the journalLines from the journalLines navigation property.

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
GET /financials/companies/{companyId}/journals/{journalId}/journalLines
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
If successful, this method returns a `200 OK` response code and a collection of [journalLine](../resources/journalline.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_journalline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/journals/{journalId}/journalLines
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.journalline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.journalLine",
      "id": "97d851da-51da-97d8-da51-d897da51d897",
      "journalDisplayName": "Journal Display Name value",
      "lineNumber": 10,
      "accountId": "ca9f694c-694c-ca9f-4c69-9fca4c699fca",
      "accountNumber": "Account Number value",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "externalDocumentNumber": "External Document Number value",
      "amount": "4.2",
      "description": "Description value",
      "comment": "Comment value",
      "lastModifiedDateTime": "2016-12-31T23:57:15.6201185+03:00"
    }
  ]
}
```


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
GET /financials/companies/{companyId}/journalLines
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
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
GET https://graph.microsoft.com/localtest/financials/companies/{companyId}/journalLines
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
      "id": "f2d18712-8712-f2d1-1287-d1f21287d1f2",
      "journalDisplayName": "Journal Display Name value",
      "lineNumber": 10,
      "accountId": "16975858-5858-1697-5858-971658589716",
      "accountNumber": "Account Number value",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "externalDocumentNumber": "External Document Number value",
      "amount": "4.2",
      "description": "Description value",
      "comment": "Comment value",
      "lastModifiedDateTime": "2016-12-31T23:58:21.1327021+03:00"
    }
  ]
}
```


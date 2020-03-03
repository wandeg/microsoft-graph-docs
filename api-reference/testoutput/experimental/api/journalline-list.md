---
title: "List journalLines"
description: "List properties and relationships of the journalLine objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List journalLines

Namespace: microsoft.graph

List properties and relationships of the [journalLine](../resources/journalline.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /financials/companies/{companyId}/journalLines
GET /financials/companies/{companyId}/journals/{journalId}/journalLines
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [journalLine](../resources/journalline.md) objects in the response body.

## Example

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
      "id": "55327cde-7cde-5532-de7c-3255de7c3255",
      "journalDisplayName": "Journal Display Name value",
      "lineNumber": 10,
      "accountId": "95554513-4513-9555-1345-559513455595",
      "accountNumber": "Account Number value",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "externalDocumentNumber": "External Document Number value",
      "amount": "4.2",
      "description": "Description value",
      "comment": "Comment value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
    }
  ]
}
```


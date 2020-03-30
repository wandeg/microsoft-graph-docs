---
title: "Get journalLine"
description: "Read properties and relationships of the journalLine object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get journalLine

Namespace: microsoft.graph

Read properties and relationships of the [journalLine](../resources/journalline.md) object.

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
GET /financials/companies/{companyId}/journalLines/{journalLineId}
GET /financials/companies/{companyId}/journals/{journalId}/journalLines/{journalLineId}
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
If successful, this method returns a `200 OK` response code and [journalLine](../resources/journalline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_journalline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/journalLines/{journalLineId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.journalLine"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 612

{
  "value": {
    "@odata.type": "#microsoft.graph.journalLine",
    "id": "e896681a-681a-e896-1a68-96e81a6896e8",
    "journalDisplayName": "Journal Display Name value",
    "lineNumber": 10,
    "accountId": "7c4a388a-388a-7c4a-8a38-4a7c8a384a7c",
    "accountNumber": "Account Number value",
    "postingDate": "Date",
    "documentNumber": "Document Number value",
    "externalDocumentNumber": "External Document Number value",
    "amount": "4.2",
    "description": "Description value",
    "comment": "Comment value",
    "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
  }
}
```


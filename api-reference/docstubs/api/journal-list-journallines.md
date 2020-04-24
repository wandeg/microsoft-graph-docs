---
title: "List journalLines"
description: "Get the journalLines from the journalLines navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List journalLines

Namespace: microsoft.graph

Get the journalLines from the journalLines navigation property.

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
GET /financials/companies/{companyId}/journals/{journalId}/journalLines
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
If successful, this method returns a `200 OK` response code and a collection of [journalLine](../resources/journalline.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_journalline"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/journals/{journalId}/journalLines
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.journalline)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.journalLine",
      "id": "12c6ff2f-ff2f-12c6-2fff-c6122fffc612",
      "journalDisplayName": "Journal Display Name value",
      "lineNumber": 10,
      "accountId": "157ed6fe-d6fe-157e-fed6-7e15fed67e15",
      "accountNumber": "Account Number value",
      "postingDate": "Date",
      "documentNumber": "Document Number value",
      "externalDocumentNumber": "External Document Number value",
      "amount": "4.2",
      "description": "Description value",
      "comment": "Comment value",
      "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
    }
  ]
}
```


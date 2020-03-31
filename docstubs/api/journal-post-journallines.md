---
title: "Add journalLines"
description: "Add journalLines by posting to the journalLines collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add journalLines

Namespace: microsoft.graph

Add journalLines by posting to the journalLines collection.

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
POST /financials/companies/{companyId}/journals/{journalId}/journalLines/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [journalLine](../resources/journalline.md) object.

The following table shows the properties that are required when you create the [journalLine](../resources/journalline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String||
|lineNumber|Int32||
|accountId|Guid||
|accountNumber|String||
|postingDate|Date||
|documentNumber|String||
|externalDocumentNumber|String||
|amount|Decimal||
|description|String||
|comment|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [journalLine](../resources/journalline.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_journalline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/journals/{journalId}/journalLines
Content-type: application/json
Content-length: 454

{
  "@odata.type": "#microsoft.graph.journalLine",
  "journalDisplayName": "Journal Display Name value",
  "lineNumber": 10,
  "accountId": "9b2499a0-99a0-9b24-a099-249ba099249b",
  "accountNumber": "Account Number value",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "externalDocumentNumber": "External Document Number value",
  "amount": "4.2",
  "description": "Description value",
  "comment": "Comment value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.journalline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.journalLine",
  "id": "2b1be251-e251-2b1b-51e2-1b2b51e21b2b",
  "journalDisplayName": "Journal Display Name value",
  "lineNumber": 10,
  "accountId": "9b2499a0-99a0-9b24-a099-249ba099249b",
  "accountNumber": "Account Number value",
  "postingDate": "Date",
  "documentNumber": "Document Number value",
  "externalDocumentNumber": "External Document Number value",
  "amount": "4.2",
  "description": "Description value",
  "comment": "Comment value",
  "lastModifiedDateTime": "2017-01-01T00:01:52.9217945+03:00"
}
```


---
title: "Create journalLines"
description: "Create a new journalLines object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create journalLines

Namespace: microsoft.graph

Create a new journalLines object.

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
POST /financials/companies/{companyId}/journalLines
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [journalLine](../resources/journalline.md) object.

The following table shows the properties that are required when you create the [journalLine](../resources/journalline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|journalDisplayName|String|**TODO: Add Description**|
|lineNumber|Int32|**TODO: Add Description**|
|accountId|Guid|**TODO: Add Description**|
|accountNumber|String|**TODO: Add Description**|
|postingDate|Date|**TODO: Add Description**|
|documentNumber|String|**TODO: Add Description**|
|externalDocumentNumber|String|**TODO: Add Description**|
|amount|Decimal|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|comment|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [journalLine](../resources/journalline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_journalline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/journalLines
Content-Type: application/json
Content-length: 454

{
  "@odata.type": "#microsoft.graph.journalLine",
  "journalDisplayName": "Journal Display Name value",
  "lineNumber": 10,
  "accountId": "157ed6fe-d6fe-157e-fed6-7e15fed67e15",
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
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.journalline"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
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
```


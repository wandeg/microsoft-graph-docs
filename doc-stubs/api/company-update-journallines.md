---
title: "Update journalLines"
description: "Update the properties of a journalLines object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update journalLines

Namespace: microsoft.graph

Update the properties of a journalLines object.

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
PATCH /financials/companies/{companyId}/journalLines
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

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

If successful, this method returns a `200 OK` response code and an updated [journalLine](../resources/journalline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_journallines"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/journalLines
Content-Type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.journalLine",
  "journalDisplayName": "String",
  "lineNumber": "Integer",
  "accountId": "Guid",
  "accountNumber": "String",
  "postingDate": "Date",
  "documentNumber": "String",
  "externalDocumentNumber": "String",
  "amount": "Decimal",
  "description": "String",
  "comment": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.journalLine",
  "id": "6aec95f0-95f0-6aec-f095-ec6af095ec6a",
  "journalDisplayName": "String",
  "lineNumber": "Integer",
  "accountId": "Guid",
  "accountNumber": "String",
  "postingDate": "Date",
  "documentNumber": "String",
  "externalDocumentNumber": "String",
  "amount": "Decimal",
  "description": "String",
  "comment": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```


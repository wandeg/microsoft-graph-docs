---
title: "Create journals"
description: "Create a new journals object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create journals

Namespace: microsoft.graph

Create a new journals object.

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
POST /financials/companies/{companyId}/journals
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [journal](../resources/journal.md) object.

The following table shows the properties that are required when you create the [journal](../resources/journal.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|code|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|balancingAccountId|Guid|**TODO: Add Description**|
|balancingAccountNumber|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [journal](../resources/journal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_journal_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/journals
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.journal",
  "code": "String",
  "displayName": "String",
  "balancingAccountId": "Guid",
  "balancingAccountNumber": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.journal"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.journal",
  "id": "1a7a94a6-94a6-1a7a-a694-7a1aa6947a1a",
  "code": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "balancingAccountId": "Guid",
  "balancingAccountNumber": "String"
}
```


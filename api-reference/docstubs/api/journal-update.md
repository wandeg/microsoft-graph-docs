---
title: "Update journal"
description: "Update the properties of a journal object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update journal

Namespace: microsoft.graph

Update the properties of a [journal](../resources/journal.md) object.

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
PATCH /financials/companies/{companyId}/journals/{journalId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `200 OK` response code and an updated [journal](../resources/journal.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_journal"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/journals/{journalId}
Content-Type: application/json
Content-length: 242

{
  "@odata.type": "#microsoft.graph.journal",
  "code": "Code value",
  "displayName": "Display Name value",
  "balancingAccountId": "533bbec1-bec1-533b-c1be-3b53c1be3b53",
  "balancingAccountNumber": "Balancing Account Number value"
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
  "@odata.type": "#microsoft.graph.journal",
  "id": "0328afd9-afd9-0328-d9af-2803d9af2803",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "balancingAccountId": "533bbec1-bec1-533b-c1be-3b53c1be3b53",
  "balancingAccountNumber": "Balancing Account Number value"
}
```


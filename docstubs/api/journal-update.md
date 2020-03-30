---
title: "Update journal"
description: "Update the properties of a journal object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update journal

Namespace: microsoft.graph

Update the properties of a [journal](../resources/journal.md) object.

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
PATCH /financials/companies/{companyId}/journals/{journalId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [journal](../resources/journal.md) object.

The following table shows the properties that are required when you create the [journal](../resources/journal.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|lastModifiedDateTime|DateTimeOffset||
|balancingAccountId|Guid||
|balancingAccountNumber|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [journal](../resources/journal.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_journal"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/journals/{journalId}
Content-type: application/json
Content-length: 242

{
  "@odata.type": "#microsoft.graph.journal",
  "code": "Code value",
  "displayName": "Display Name value",
  "balancingAccountId": "b0bf1d30-1d30-b0bf-301d-bfb0301dbfb0",
  "balancingAccountNumber": "Balancing Account Number value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.journal",
  "id": "1de974c4-74c4-1de9-c474-e91dc474e91d",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00",
  "balancingAccountId": "b0bf1d30-1d30-b0bf-301d-bfb0301dbfb0",
  "balancingAccountNumber": "Balancing Account Number value"
}
```


---
title: "Add journals"
description: "Add journals by posting to the journals collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add journals

Namespace: microsoft.graph

Add journals by posting to the journals collection.

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
POST /financials/companies/{companyId}/journals/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [journal](../resources/journal.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_journal_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies/{companyId}/journals
Content-type: application/json
Content-length: 242

{
  "@odata.type": "#microsoft.graph.journal",
  "code": "Code value",
  "displayName": "Display Name value",
  "balancingAccountId": "4d5af2d7-f2d7-4d5a-d7f2-5a4dd7f25a4d",
  "balancingAccountNumber": "Balancing Account Number value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.journal"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 355

{
  "@odata.type": "#microsoft.graph.journal",
  "id": "81513f0e-3f0e-8151-0e3f-51810e3f5181",
  "code": "Code value",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "balancingAccountId": "4d5af2d7-f2d7-4d5a-d7f2-5a4dd7f25a4d",
  "balancingAccountNumber": "Balancing Account Number value"
}
```


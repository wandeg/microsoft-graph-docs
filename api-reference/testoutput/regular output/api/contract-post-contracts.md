---
title: "Create contract"
description: "Create a new contract object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create contract

Namespace: microsoft.graph

Create a new [contract](../resources/contract.md) object.

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
POST /contracts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [contract](../resources/contract.md) object.

The following table shows the properties that are required when you create the [contract](../resources/contract.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset| Inherited from [directoryObject](../resources/directoryobject.md)|
|contractType|String||
|customerId|Guid||
|defaultDomainName|String||
|displayName|String||



## Response
If successful, this method returns a `201 Created` response code and a [contract](../resources/contract.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_contract_from_contracts"
}
-->
``` http
POST https://graph.microsoft.com/localtest/contracts
Content-type: application/json
Content-length: 301

{
  "@odata.type": "#microsoft.graph.contract",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
  "contractType": "Contract Type value",
  "customerId": "c0ee7d7f-7d7f-c0ee-7f7d-eec07f7deec0",
  "defaultDomainName": "Default Domain Name value",
  "displayName": "Display Name value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 350

{
  "@odata.type": "#microsoft.graph.contract",
  "id": "0a8b661a-661a-0a8b-1a66-8b0a1a668b0a",
  "deletedDateTime": "2016-12-31T23:58:21.3371057+03:00",
  "contractType": "Contract Type value",
  "customerId": "c0ee7d7f-7d7f-c0ee-7f7d-eec07f7deec0",
  "defaultDomainName": "Default Domain Name value",
  "displayName": "Display Name value"
}
```


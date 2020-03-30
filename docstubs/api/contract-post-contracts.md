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
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
POST https://graph.microsoft.com/beta/contracts
Content-type: application/json
Content-length: 301

{
  "@odata.type": "#microsoft.graph.contract",
  "deletedDateTime": "2016-12-31T23:57:00.1067265+03:00",
  "contractType": "Contract Type value",
  "customerId": "9d8a53f3-53f3-9d8a-f353-8a9df3538a9d",
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
  "id": "4de33d62-3d62-4de3-623d-e34d623de34d",
  "deletedDateTime": "2016-12-31T23:57:00.1067265+03:00",
  "contractType": "Contract Type value",
  "customerId": "9d8a53f3-53f3-9d8a-f353-8a9df3538a9d",
  "defaultDomainName": "Default Domain Name value",
  "displayName": "Display Name value"
}
```


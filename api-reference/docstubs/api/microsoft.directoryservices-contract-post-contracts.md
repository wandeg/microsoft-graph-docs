---
title: "Create contract"
description: "Create a new contract object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create contract

Namespace: Microsoft.DirectoryServices

Create a new [contract](../resources/microsoft.directoryservices-contract.md) object.

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
POST /contracts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [contract](../resources/microsoft.directoryservices-contract.md) object.

The following table shows the properties that are required when you create the [contract](../resources/microsoft.directoryservices-contract.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/microsoft.directoryservices-directoryobject.md)|
|contractType|String|**TODO: Add Description**|
|customerId|Guid|**TODO: Add Description**|
|defaultDomainName|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [contract](../resources/microsoft.directoryservices-contract.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_contract_from_contracts"
}
-->
``` http
POST https://graph.microsoft.com/changelog/contracts
Content-Type: application/json
Content-length: 313

{
  "@odata.type": "#Microsoft.DirectoryServices.contract",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "contractType": "Contract Type value",
  "customerId": "9e2e4aa1-4aa1-9e2e-a14a-2e9ea14a2e9e",
  "defaultDomainName": "Default Domain Name value",
  "displayName": "Display Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.directoryservices.contract"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.contract",
  "id": "1a733748-3748-1a73-4837-731a4837731a",
  "deletedDateTime": "2016-12-31T23:59:35.6179565+00:00",
  "contractType": "Contract Type value",
  "customerId": "9e2e4aa1-4aa1-9e2e-a14a-2e9ea14a2e9e",
  "defaultDomainName": "Default Domain Name value",
  "displayName": "Display Name value"
}
```


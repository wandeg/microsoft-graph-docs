---
title: "Update tokenLifetimePolicy"
description: "Update the properties of a tokenLifetimePolicy object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update tokenLifetimePolicy

Namespace: Microsoft.DirectoryServices

Update the properties of a [tokenLifetimePolicy](../resources/microsoft.directoryservices-tokenlifetimepolicy.md) object.

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
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [tokenLifetimePolicy](../resources/microsoft.directoryservices-tokenlifetimepolicy.md) object.

The following table shows the properties that are required when you create the [tokenLifetimePolicy](../resources/microsoft.directoryservices-tokenlifetimepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/microsoft.directoryservices-policybase.md)|
|definition|String collection|**TODO: Add Description** Inherited from [stsPolicy](../resources/microsoft.directoryservices-stspolicy.md)|
|isOrganizationDefault|Boolean|**TODO: Add Description** Inherited from [stsPolicy](../resources/microsoft.directoryservices-stspolicy.md)|



## Response
If successful, this method returns a `200 OK` response code and an updated [tokenLifetimePolicy](../resources/microsoft.directoryservices-tokenlifetimepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_tokenlifetimepolicy"
}
-->
``` http

```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.DirectoryServices.tokenLifetimePolicy",
  "id": "b34e4c79-4c79-b34e-794c-4eb3794c4eb3",
  "description": "Description value",
  "displayName": "Display Name value",
  "definition": [
    "Definition value"
  ],
  "isOrganizationDefault": true
}
```


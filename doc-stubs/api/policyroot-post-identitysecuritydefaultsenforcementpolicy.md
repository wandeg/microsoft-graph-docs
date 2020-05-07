---
title: "Create identitySecurityDefaultsEnforcementPolicy"
description: "Create a new identitySecurityDefaultsEnforcementPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create identitySecurityDefaultsEnforcementPolicy

Namespace: microsoft.graph

Create a new identitySecurityDefaultsEnforcementPolicy object.

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
POST /policies/identitySecurityDefaultsEnforcementPolicy
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object.

The following table shows the properties that are required when you create the [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|description|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|displayName|String|**TODO: Add Description** Inherited from [policyBase](../resources/policybase.md)|
|isEnabled|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_identitysecuritydefaultsenforcementpolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
Content-Type: application/json
Content-length: 210

{
  "@odata.type": "#microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identitysecuritydefaultsenforcementpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
  "id": "25a3f67f-f67f-25a3-7ff6-a3257ff6a325",
  "deletedDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean"
}
```


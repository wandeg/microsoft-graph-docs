---
title: "Update identitySecurityDefaultsEnforcementPolicy"
description: "Update the properties of an identitySecurityDefaultsEnforcementPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update identitySecurityDefaultsEnforcementPolicy

Namespace: microsoft.graph

Update the properties of an identitySecurityDefaultsEnforcementPolicy object.

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
PATCH /policies/identitySecurityDefaultsEnforcementPolicy
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

If successful, this method returns a `200 OK` response code and an updated [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_identitysecuritydefaultsenforcementpolicy"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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


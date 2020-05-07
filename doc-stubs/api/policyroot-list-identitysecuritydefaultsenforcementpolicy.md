---
title: "List identitySecurityDefaultsEnforcementPolicy"
description: "Get the identitySecurityDefaultsEnforcementPolicies from the identitySecurityDefaultsEnforcementPolicy navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List identitySecurityDefaultsEnforcementPolicy

Namespace: microsoft.graph

Get the identitySecurityDefaultsEnforcementPolicies from the identitySecurityDefaultsEnforcementPolicy navigation property.

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
GET /policies/identitySecurityDefaultsEnforcementPolicy
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [identitySecurityDefaultsEnforcementPolicy](../resources/identitysecuritydefaultsenforcementpolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_identitysecuritydefaultsenforcementpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/identitySecurityDefaultsEnforcementPolicy
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.identitysecuritydefaultsenforcementpolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.identitySecurityDefaultsEnforcementPolicy",
      "id": "25a3f67f-f67f-25a3-7ff6-a3257ff6a325",
      "deletedDateTime": "String (timestamp)",
      "description": "String",
      "displayName": "String",
      "isEnabled": "Boolean"
    }
  ]
}
```


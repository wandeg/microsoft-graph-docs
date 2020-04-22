---
title: "Get claimsMappingPolicy"
description: "Read properties and relationships of a claimsMappingPolicy object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Get claimsMappingPolicy

Namespace: microsoft.graph

Read properties and relationships of a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object.

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
GET /policies/claimsMappingPolicies/{claimsMappingPolicyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_claimsmappingpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{claimsMappingPolicyId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.claimsMappingPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.claimsMappingPolicy",
    "id": "76095785-5785-7609-8557-097685570976",
    "description": "Description value",
    "displayName": "Display Name value",
    "definition": [
      "Definition value"
    ],
    "isOrganizationDefault": true
  }
}
```


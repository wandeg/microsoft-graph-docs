---
title: "Get homeRealmDiscoveryPolicy"
description: "Read properties and relationships of the homeRealmDiscoveryPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get homeRealmDiscoveryPolicy

Namespace: microsoft.graph

Read properties and relationships of the [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object.

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
GET /policies/homeRealmDiscoveryPolicies/{homeRealmDiscoveryPolicyId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_homerealmdiscoverypolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{homeRealmDiscoveryPolicyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.homeRealmDiscoveryPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 312

{
  "value": {
    "@odata.type": "#microsoft.graph.homeRealmDiscoveryPolicy",
    "id": "f31cb23b-b23b-f31c-3bb2-1cf33bb21cf3",
    "description": "Description value",
    "displayName": "Display Name value",
    "definition": [
      "Definition value"
    ],
    "isOrganizationDefault": true
  }
}
```


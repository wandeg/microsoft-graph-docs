---
title: "Get tokenLifetimePolicy"
description: "Read properties and relationships of the tokenLifetimePolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get tokenLifetimePolicy

Namespace: microsoft.graph

Read properties and relationships of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.

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
GET /policies/tokenLifetimePolicies/{tokenLifetimePolicyId}
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
If successful, this method returns a `200 OK` response code and [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/{tokenLifetimePolicyId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 307

{
  "value": {
    "@odata.type": "#microsoft.graph.tokenLifetimePolicy",
    "id": "4b8bf866-f866-4b8b-66f8-8b4b66f88b4b",
    "description": "Description value",
    "displayName": "Display Name value",
    "definition": [
      "Definition value"
    ],
    "isOrganizationDefault": true
  }
}
```


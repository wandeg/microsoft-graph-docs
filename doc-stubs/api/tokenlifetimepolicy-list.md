---
title: "List tokenLifetimePolicies"
description: "Get a list of the tokenLifetimePolicy objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List tokenLifetimePolicies
Namespace: microsoft.graph

Get a list of the [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects and their properties.

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
GET /policies/tokenLifetimePolicies
GET /applications/{applicationsId}/tokenLifetimePolicies
GET /servicePrincipals/{servicePrincipalsId}/tokenLifetimePolicies
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

If successful, this method returns a `200 OK` response code and a collection of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_tokenlifetimepolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.tokenlifetimepolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tokenLifetimePolicy",
      "id": "96f4f5a4-f5a4-96f4-a4f5-f496a4f5f496",
      "deletedDateTime": "String (timestamp)",
      "description": "String",
      "displayName": "String",
      "definition": [
        "String"
      ],
      "isOrganizationDefault": "Boolean"
    }
  ]
}
```


---
title: "List scopedRoleMemberships"
description: "Get a list of the scopedRoleMembership objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List scopedRoleMemberships

Namespace: microsoft.graph

Get a list of the [scopedRoleMembership](../resources/scopedrolemembership.md) objects and their properties.

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
GET /scopedRoleMemberships
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
If successful, this method returns a `200 OK` response code and a collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemembership"
}
-->
``` http
GET https://graph.microsoft.com/beta/scopedRoleMemberships
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.scopedrolemembership)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.scopedRoleMembership",
      "id": "47b938e2-38e2-47b9-e238-b947e238b947",
      "roleId": "Role Id value",
      "administrativeUnitId": "Administrative Unit Id value",
      "roleMemberInfo": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value",
        "displayName": "Display Name value"
      }
    }
  ]
}
```


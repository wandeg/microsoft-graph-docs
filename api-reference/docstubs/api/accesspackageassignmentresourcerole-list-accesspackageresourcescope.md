---
title: "List accessPackageResourceScope"
description: "Get the accessPackageResourceScopes from the accessPackageResourceScope navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessPackageResourceScope

Namespace: microsoft.graph

Get the accessPackageResourceScopes from the accessPackageResourceScope navigation property.

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
GET /accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageResourceScope
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
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResourceScope](../resources/accesspackageresourcescope.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresourcescope"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageAssignmentResourceRoles/{accessPackageAssignmentResourceRolesId}/accessPackageResourceScope
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageresourcescope)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResourceScope",
      "id": "175a2647-2647-175a-4726-5a1747265a17",
      "displayName": "Display Name value",
      "description": "Description value",
      "originId": "Origin Id value",
      "originSystem": "Origin System value",
      "roleOriginId": "Role Origin Id value",
      "isRootScope": true,
      "url": "Url value"
    }
  ]
}
```


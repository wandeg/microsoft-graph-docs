---
title: "List accessPackageResource"
description: "Get the accessPackageResources from the accessPackageResource navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessPackageResource

Namespace: microsoft.graph

Get the accessPackageResources from the accessPackageResource navigation property.

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
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceRoles/{accessPackageResourceRoleId}/accessPackageResource
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
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceRoles/{accessPackageResourceRoleId}/accessPackageResource
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageresource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResource",
      "id": "e8e4902b-902b-e8e4-2b90-e4e82b90e4e8",
      "displayName": "Display Name value",
      "description": "Description value",
      "url": "Url value",
      "resourceType": "Resource Type value",
      "originId": "Origin Id value",
      "originSystem": "Origin System value",
      "isPendingOnboarding": true,
      "addedBy": "Added By value",
      "addedOn": "2016-12-31T23:57:56.5735419+03:00"
    }
  ]
}
```


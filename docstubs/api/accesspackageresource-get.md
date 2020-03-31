---
title: "Get accessPackageResource"
description: "Read properties and relationships of the accessPackageResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get accessPackageResource

Namespace: microsoft.graph

Read properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) object.

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
GET /accessPackageResources/{accessPackageResourcesId}
GET /identityGovernance/entitlementManagement/accessPackageResources/{accessPackageResourceId}
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResources/{accessPackageResourceId}
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceRoles/{accessPackageResourceRoleId}/accessPackageResource
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources/{accessPackageResourceId}/accessPackageResourceScopes/{accessPackageResourceScopeId}/accessPackageResource
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
If successful, this method returns a `200 OK` response code and [accessPackageResource](../resources/accesspackageresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageResources/{accessPackageResourcesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 488

{
  "value": {
    "@odata.type": "#microsoft.graph.accessPackageResource",
    "id": "dd11afa0-afa0-dd11-a0af-11dda0af11dd",
    "displayName": "Display Name value",
    "description": "Description value",
    "url": "Url value",
    "resourceType": "Resource Type value",
    "originId": "Origin Id value",
    "originSystem": "Origin System value",
    "isPendingOnboarding": true,
    "addedBy": "Added By value",
    "addedOn": "2016-12-31T23:57:24.4546609+03:00"
  }
}
```


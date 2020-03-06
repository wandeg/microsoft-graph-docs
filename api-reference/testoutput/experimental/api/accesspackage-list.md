---
title: "List accessPackages"
description: "List properties and relationships of the accessPackage objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackages

Namespace: microsoft.graph

List properties and relationships of the [accessPackage](../resources/accesspackage.md) objects.

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
GET /accessPackages
GET /identityGovernance/entitlementManagement/accessPackages
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackages
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}
-->
``` http
GET https://graph.microsoft.com/localtest/accessPackages
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 542

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackage",
      "id": "931941b8-41b8-9319-b841-1993b8411993",
      "catalogId": "Catalog Id value",
      "displayName": "Display Name value",
      "description": "Description value",
      "isHidden": true,
      "isRoleScopesVisible": true,
      "createdBy": "Created By value",
      "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2016-12-31T23:58:13.3996216+03:00"
    }
  ]
}
```


---
title: "List accessPackageResources"
description: "List properties and relationships of the accessPackageResource objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List accessPackageResources

Namespace: microsoft.graph

List properties and relationships of the [accessPackageResource](../resources/accesspackageresource.md) objects.

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
GET /accessPackageResources
GET /identityGovernance/entitlementManagement/accessPackageResources
GET /accessPackageCatalogs/{accessPackageCatalogsId}/accessPackageResources
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackageResources
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
If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackageResources
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackageresource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 524

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageResource",
      "id": "fa3fefe2-efe2-fa3f-e2ef-3ffae2ef3ffa",
      "displayName": "Display Name value",
      "description": "Description value",
      "url": "Url value",
      "resourceType": "Resource Type value",
      "originId": "Origin Id value",
      "originSystem": "Origin System value",
      "isPendingOnboarding": true,
      "addedBy": "Added By value",
      "addedOn": "2016-12-31T23:57:56.6124592+03:00"
    }
  ]
}
```


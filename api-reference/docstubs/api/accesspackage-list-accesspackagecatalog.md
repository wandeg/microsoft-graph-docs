---
title: "List accessPackageCatalog"
description: "Get the accessPackageCatalogs from the accessPackageCatalog navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessPackageCatalog

Namespace: microsoft.graph

Get the accessPackageCatalogs from the accessPackageCatalog navigation property.

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
GET /accessPackages/{accessPackagesId}/accessPackageCatalog
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
If successful, this method returns a `200 OK` response code and a collection of [accessPackageCatalog](../resources/accesspackagecatalog.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}
-->
``` http
GET https://graph.microsoft.com/beta/accessPackages/{accessPackagesId}/accessPackageCatalog
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accesspackagecatalog)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackageCatalog",
      "id": "ed0dcd9e-cd9e-ed0d-9ecd-0ded9ecd0ded",
      "displayName": "Display Name value",
      "description": "Description value",
      "catalogType": "Catalog Type value",
      "catalogStatus": "Catalog Status value",
      "isExternallyVisible": true,
      "createdBy": "Created By value",
      "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
      "modifiedBy": "Modified By value",
      "modifiedDateTime": "2017-01-01T00:00:03.7977786+03:00"
    }
  ]
}
```


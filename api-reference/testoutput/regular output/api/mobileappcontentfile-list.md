---
title: "List mobileAppContentFiles"
description: "List properties and relationships of the mobileAppContentFile objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mobileAppContentFiles

Namespace: microsoft.graph

List properties and relationships of the [mobileAppContentFile](../resources/mobileappcontentfile.md) objects.

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
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mobileAppContentFile](../resources/mobileappcontentfile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobileappcontentfile"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mobileappcontentfile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 519

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppContentFile",
      "id": "2e15890d-890d-2e15-0d89-152e0d89152e",
      "azureStorageUri": "Azure Storage Uri value",
      "isCommitted": true,
      "createdDateTime": "2017-01-01T00:00:31.7073518+03:00",
      "name": "Name value",
      "size": 4,
      "sizeEncrypted": 13,
      "azureStorageUriExpirationDateTime": "2016-12-31T23:59:18.2738909+03:00",
      "manifest": "bWFuaWZlc3Q=",
      "uploadState": "String"
    }
  ]
}
```


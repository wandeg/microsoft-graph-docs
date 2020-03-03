---
title: "List managedEBookCategories"
description: "List properties and relationships of the managedEBookCategory objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List managedEBookCategories

Namespace: microsoft.graph

List properties and relationships of the [managedEBookCategory](../resources/managedebookcategory.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [managedEBookCategory](../resources/managedebookcategory.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_managedebookcategory"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/managedEBookCategories
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.managedebookcategory)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookCategory",
      "id": "75c9c15e-c15e-75c9-5ec1-c9755ec1c975",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00"
    }
  ]
}
```


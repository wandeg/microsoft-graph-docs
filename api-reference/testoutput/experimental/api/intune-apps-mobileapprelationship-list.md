---
title: "List mobileAppRelationships"
description: "List properties and relationships of the mobileAppRelationship objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List mobileAppRelationships

Namespace: microsoft.graph

List properties and relationships of the [mobileAppRelationship](../resources/mobileapprelationship.md) objects.

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
GET /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [mobileAppRelationship](../resources/mobileapprelationship.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_mobileapprelationship"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.mobileapprelationship)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 248

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppRelationship",
      "id": "680e718a-718a-680e-8a71-0e688a710e68",
      "targetId": "Target Id value",
      "targetDisplayName": "Target Display Name value"
    }
  ]
}
```


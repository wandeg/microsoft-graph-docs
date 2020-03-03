---
title: "List locationManagementConditions"
description: "List properties and relationships of the locationManagementCondition objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List locationManagementConditions

Namespace: microsoft.graph

List properties and relationships of the [locationManagementCondition](../resources/locationmanagementcondition.md) objects.

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
GET ** Collection URI for microsoft.graph.locationManagementCondition not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [locationManagementCondition](../resources/locationmanagementcondition.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_locationmanagementcondition"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.locationManagementCondition not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.locationmanagementcondition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.locationManagementCondition",
      "id": "ccec6d9f-6d9f-ccec-9f6d-eccc9f6deccc",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
      "modifiedDateTime": "2016-12-31T23:56:57.1102355+03:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "String"
      ]
    }
  ]
}
```


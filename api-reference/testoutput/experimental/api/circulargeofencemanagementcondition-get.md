---
title: "Get circularGeofenceManagementCondition"
description: "Read properties and relationships of the circularGeofenceManagementCondition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get circularGeofenceManagementCondition

Read properties and relationships of the [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) object.

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
GET ** Entity URI for microsoft.graph.circularGeofenceManagementCondition not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_circulargeofencemanagementcondition"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.circularGeofenceManagementCondition not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.circularGeofenceManagementCondition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 564

{
  "value": {
    "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
    "id": "85edb7d1-b7d1-85ed-d1b7-ed85d1b7ed85",
    "uniqueName": "Unique Name value",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
    "modifiedDateTime": "2017-01-01T00:03:12.7204145+03:00",
    "eTag": "ETag value",
    "applicablePlatforms": [
      "String"
    ],
    "latitude": "Double",
    "longitude": "Double",
    "radiusInMeters": "Single"
  }
}
```


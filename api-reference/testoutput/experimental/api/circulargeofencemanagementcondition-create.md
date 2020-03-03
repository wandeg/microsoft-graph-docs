---
title: "Create circularGeofenceManagementCondition"
description: "Create a new circularGeofenceManagementCondition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create circularGeofenceManagementCondition

Create a new [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) object.

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
POST ** Collection URI for microsoft.graph.circularGeofenceManagementCondition not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the circularGeofenceManagementCondition object.

The following table shows the properties that are required when you create the circularGeofenceManagementCondition.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|uniqueName|String|Unique name for the management condition. Used in management condition expressions. Inherited from [managementCondition](../resources/managementCondition.md)|
|displayName|String|The admin defined name of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|description|String|The admin defined description of the management condition. Inherited from [managementCondition](../resources/managementCondition.md)|
|createdDateTime|DateTimeOffset|The time the management condition was created. Generated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|modifiedDateTime|DateTimeOffset|The time the management condition was last modified. Updated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|eTag|String|ETag of the management condition. Updated service side. Inherited from [managementCondition](../resources/managementCondition.md)|
|applicablePlatforms|Enumeration collection|The applicable platforms for this management condition. Inherited from [managementCondition](../resources/managementCondition.md). Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|latitude|Double|Latitude in degrees, between -90 and +90 inclusive.|
|longitude|Double|Longitude in degrees, between -180 and +180 inclusive.|
|radiusInMeters|Single|Radius in meters.|



## Response
If successful, this method returns a `201 Created` response code and a [circularGeofenceManagementCondition](../resources/circulargeofencemanagementcondition.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_circulargeofencemanagementcondition_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.circularGeofenceManagementCondition not found
Content-type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.circularGeofenceManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "String"
  ],
  "latitude": "Double",
  "longitude": "Double",
  "radiusInMeters": "Single"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.circulargeofencemanagementcondition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 517

{
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
```


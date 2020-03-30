---
title: "Get windowsFeatureUpdateProfileAssignment"
description: "Read properties and relationships of the windowsFeatureUpdateProfileAssignment object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsFeatureUpdateProfileAssignment

Namespace: microsoft.graph

Read properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md) object.

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
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
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
If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfileAssignment](../resources/windowsfeatureupdateprofileassignment.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsfeatureupdateprofileassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsFeatureUpdateProfileAssignment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
    "id": "9caa54c8-54c8-9caa-c854-aa9cc854aa9c",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```


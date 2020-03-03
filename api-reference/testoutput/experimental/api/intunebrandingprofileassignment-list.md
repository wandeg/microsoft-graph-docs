---
title: "List intuneBrandingProfileAssignments"
description: "List properties and relationships of the intuneBrandingProfileAssignment objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List intuneBrandingProfileAssignments

Namespace: microsoft.graph

List properties and relationships of the [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) objects.

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
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [intuneBrandingProfileAssignment](../resources/intunebrandingprofileassignment.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_intunebrandingprofileassignment"
}
-->
``` http
GET https://graph.microsoft.com/localtest/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.intunebrandingprofileassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 273

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
      "id": "c3f71358-1358-c3f7-5813-f7c35813f7c3",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```


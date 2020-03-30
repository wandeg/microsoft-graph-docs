---
title: "Get appleUserInitiatedEnrollmentProfile"
description: "Read properties and relationships of the appleUserInitiatedEnrollmentProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get appleUserInitiatedEnrollmentProfile

Namespace: microsoft.graph

Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object.

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
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
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
If successful, this method returns a `200 OK` response code and [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_appleuserinitiatedenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appleUserInitiatedEnrollmentProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 653

{
  "value": {
    "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
    "id": "19f90199-0199-19f9-9901-f9199901f919",
    "defaultEnrollmentType": "String",
    "availableEnrollmentTypeOptions": [
      {
        "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
        "ownerType": "String",
        "enrollmentType": "String"
      }
    ],
    "displayName": "Display Name value",
    "description": "Description value",
    "priority": 8,
    "platform": "String",
    "createdDateTime": "2017-01-01T00:01:44.2536508+00:00",
    "lastModifiedDateTime": "2017-01-01T00:03:05.9649885+00:00"
  }
}
```


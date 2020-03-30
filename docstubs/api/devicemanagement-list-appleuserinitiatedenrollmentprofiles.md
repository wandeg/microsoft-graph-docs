---
title: "List appleUserInitiatedEnrollmentProfiles"
description: "Get the appleUserInitiatedEnrollmentProfiles from the appleUserInitiatedEnrollmentProfiles navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appleUserInitiatedEnrollmentProfiles

Namespace: microsoft.graph

Get the appleUserInitiatedEnrollmentProfiles from the appleUserInitiatedEnrollmentProfiles navigation property.

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
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles
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
If successful, this method returns a `200 OK` response code and a collection of [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_appleuserinitiatedenrollmentprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.appleuserinitiatedenrollmentprofile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 699

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
      "id": "b0133d47-3d47-b013-473d-13b0473d13b0",
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
      "createdDateTime": "2016-12-31T23:56:52.9286964+00:00",
      "lastModifiedDateTime": "2017-01-01T00:02:50.3839766+00:00"
    }
  ]
}
```


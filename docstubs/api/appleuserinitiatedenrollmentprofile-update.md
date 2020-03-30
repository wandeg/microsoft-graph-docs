---
title: "Update appleUserInitiatedEnrollmentProfile"
description: "Update the properties of a appleUserInitiatedEnrollmentProfile object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update appleUserInitiatedEnrollmentProfile

Namespace: microsoft.graph

Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object.

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
PATCH /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object.

The following table shows the properties that are required when you create the [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|defaultEnrollmentType|Enumeration| Possible values are: `unknown`, `device`, `user`.|
|availableEnrollmentTypeOptions|[appleOwnerTypeEnrollmentType](../resources/appleownertypeenrollmenttype.md) collection||
|displayName|String||
|description|String||
|priority|Int32||
|platform|Enumeration| Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|createdDateTime|DateTimeOffset||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [appleUserInitiatedEnrollmentProfile](../resources/appleuserinitiatedenrollmentprofile.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_appleuserinitiatedenrollmentprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}
Content-type: application/json
Content-length: 430

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
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
  "platform": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 602

{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "id": "301a9b6f-9b6f-301a-6f9b-1a306f9b1a30",
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
  "createdDateTime": "2016-12-31T23:59:16.3214767+03:00",
  "lastModifiedDateTime": "2017-01-01T00:01:54.3678257+03:00"
}
```


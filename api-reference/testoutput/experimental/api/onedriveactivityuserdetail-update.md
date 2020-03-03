---
title: "Update oneDriveActivityUserDetail"
description: "Update the properties of a oneDriveActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update oneDriveActivityUserDetail

Update the properties of a [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.oneDriveActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [oneDriveActivityUserDetail](../resources/oneDriveActivityUserDetail.md) object.

The following table shows the properties that are required when you create the [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|isDeleted|Boolean||
|deletedDate|Date||
|lastActivityDate|Date||
|viewedOrEditedFileCount|Int64||
|syncedFileCount|Int64||
|sharedInternallyFileCount|Int64||
|sharedExternallyFileCount|Int64||
|assignedProducts|String collection||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_onedriveactivityuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.oneDriveActivityUserDetail not found
Content-type: application/json
Content-length: 465

{
  "@odata.type": "#microsoft.graph.oneDriveActivityUserDetail",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "viewedOrEditedFileCount": 7,
  "syncedFileCount": 15,
  "sharedInternallyFileCount": 9,
  "sharedExternallyFileCount": 9,
  "assignedProducts": [
    "Assigned Products value"
  ],
  "reportPeriod": "Report Period value"
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
Content-Length: 514

{
  "@odata.type": "#microsoft.graph.oneDriveActivityUserDetail",
  "id": "7173f9d4-f9d4-7173-d4f9-7371d4f97371",
  "reportRefreshDate": "Date",
  "userPrincipalName": "User Principal Name value",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "viewedOrEditedFileCount": 7,
  "syncedFileCount": 15,
  "sharedInternallyFileCount": 9,
  "sharedExternallyFileCount": 9,
  "assignedProducts": [
    "Assigned Products value"
  ],
  "reportPeriod": "Report Period value"
}
```


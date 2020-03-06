---
title: "getOneDriveActivityUserDetail"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOneDriveActivityUserDetail

Namespace: microsoft.graph



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
GET /reports/getOneDriveActivityUserDetail
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [oneDriveActivityUserDetail](../resources/onedriveactivityuserdetail.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest/reports/getOneDriveActivityUserDetail(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.onedriveactivityuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 607

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.oneDriveActivityUserDetail",
      "id": "4c8b2d0c-2d0c-4c8b-0c2d-8b4c0c2d8b4c",
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
  ]
}
```


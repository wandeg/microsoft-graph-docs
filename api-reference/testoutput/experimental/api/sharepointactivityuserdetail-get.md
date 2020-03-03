---
title: "Get sharePointActivityUserDetail"
description: "Read properties and relationships of the sharePointActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get sharePointActivityUserDetail

Read properties and relationships of the [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object.

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
GET ** Entity URI for microsoft.graph.sharePointActivityUserDetail not found
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
If successful, this method returns a `200 OK` response code and [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_sharepointactivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.sharePointActivityUserDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointActivityUserDetail"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 593

{
  "value": {
    "@odata.type": "#microsoft.graph.sharePointActivityUserDetail",
    "id": "35616396-6396-3561-9663-613596636135",
    "reportRefreshDate": "Date",
    "userPrincipalName": "User Principal Name value",
    "isDeleted": true,
    "deletedDate": "Date",
    "lastActivityDate": "Date",
    "viewedOrEditedFileCount": 7,
    "syncedFileCount": 15,
    "sharedInternallyFileCount": 9,
    "sharedExternallyFileCount": 9,
    "visitedPageCount": 0,
    "assignedProducts": [
      "Assigned Products value"
    ],
    "reportPeriod": "Report Period value"
  }
}
```


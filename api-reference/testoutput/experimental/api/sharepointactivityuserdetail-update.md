---
title: "Update sharePointActivityUserDetail"
description: "Update the properties of a sharePointActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update sharePointActivityUserDetail

Namespace: microsoft.graph

Update the properties of a [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.sharePointActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object.

The following table shows the properties that are required when you create the [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md).

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
|visitedPageCount|Int64||
|assignedProducts|String collection||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_sharepointactivityuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.sharePointActivityUserDetail not found
Content-type: application/json
Content-length: 493

{
  "@odata.type": "#microsoft.graph.sharePointActivityUserDetail",
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
Content-Length: 542

{
  "@odata.type": "#microsoft.graph.sharePointActivityUserDetail",
  "id": "fe712b8e-2b8e-fe71-8e2b-71fe8e2b71fe",
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
```


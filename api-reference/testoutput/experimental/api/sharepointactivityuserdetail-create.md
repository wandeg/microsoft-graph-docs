---
title: "Create sharePointActivityUserDetail"
description: "Create a new sharePointActivityUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create sharePointActivityUserDetail

Namespace: microsoft.graph

Create a new [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object.

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
POST ** Collection URI for microsoft.graph.sharePointActivityUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_sharepointactivityuserdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.sharePointActivityUserDetail not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.sharepointactivityuserdetail"
}
-->
``` http
HTTP/1.1 201 Created
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


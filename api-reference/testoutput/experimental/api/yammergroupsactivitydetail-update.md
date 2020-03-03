---
title: "Update yammerGroupsActivityDetail"
description: "Update the properties of a yammerGroupsActivityDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update yammerGroupsActivityDetail

Namespace: microsoft.graph

Update the properties of a [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.yammerGroupsActivityDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object.

The following table shows the properties that are required when you create the [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|groupDisplayName|String||
|isDeleted|Boolean||
|ownerPrincipalName|String||
|lastActivityDate|Date||
|groupType|String||
|office365Connected|Boolean||
|memberCount|Int64||
|postedCount|Int64||
|readCount|Int64||
|likedCount|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_yammergroupsactivitydetail"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.yammerGroupsActivityDetail not found
Content-type: application/json
Content-length: 452

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
  "reportRefreshDate": "Date",
  "groupDisplayName": "Group Display Name value",
  "isDeleted": true,
  "ownerPrincipalName": "Owner Principal Name value",
  "lastActivityDate": "Date",
  "groupType": "Group Type value",
  "office365Connected": true,
  "memberCount": 11,
  "postedCount": 11,
  "readCount": 9,
  "likedCount": 10,
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
Content-Length: 501

{
  "@odata.type": "#microsoft.graph.yammerGroupsActivityDetail",
  "id": "54513b00-3b00-5451-003b-5154003b5154",
  "reportRefreshDate": "Date",
  "groupDisplayName": "Group Display Name value",
  "isDeleted": true,
  "ownerPrincipalName": "Owner Principal Name value",
  "lastActivityDate": "Date",
  "groupType": "Group Type value",
  "office365Connected": true,
  "memberCount": 11,
  "postedCount": 11,
  "readCount": 9,
  "likedCount": 10,
  "reportPeriod": "Report Period value"
}
```


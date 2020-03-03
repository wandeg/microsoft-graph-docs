---
title: "Create office365GroupsActivityDetail"
description: "Create a new office365GroupsActivityDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365GroupsActivityDetail

Namespace: microsoft.graph

Create a new [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) object.

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
POST ** Collection URI for microsoft.graph.office365GroupsActivityDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) object.

The following table shows the properties that are required when you create the [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|groupId|String||
|groupDisplayName|String||
|isDeleted|Boolean||
|ownerPrincipalName|String||
|lastActivityDate|Date||
|groupType|String||
|memberCount|Int64||
|externalMemberCount|Int64||
|exchangeReceivedEmailCount|Int64||
|sharePointActiveFileCount|Int64||
|yammerPostedMessageCount|Int64||
|yammerReadMessageCount|Int64||
|yammerLikedMessageCount|Int64||
|exchangeMailboxTotalItemCount|Int64||
|exchangeMailboxStorageUsedInBytes|Int64||
|sharePointTotalFileCount|Int64||
|sharePointSiteStorageUsedInBytes|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365groupsactivitydetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.office365GroupsActivityDetail not found
Content-type: application/json
Content-length: 753

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityDetail",
  "reportRefreshDate": "Date",
  "groupId": "Group Id value",
  "groupDisplayName": "Group Display Name value",
  "isDeleted": true,
  "ownerPrincipalName": "Owner Principal Name value",
  "lastActivityDate": "Date",
  "groupType": "Group Type value",
  "memberCount": 11,
  "externalMemberCount": 3,
  "exchangeReceivedEmailCount": 10,
  "sharePointActiveFileCount": 9,
  "yammerPostedMessageCount": 8,
  "yammerReadMessageCount": 6,
  "yammerLikedMessageCount": 7,
  "exchangeMailboxTotalItemCount": 13,
  "exchangeMailboxStorageUsedInBytes": 1,
  "sharePointTotalFileCount": 8,
  "sharePointSiteStorageUsedInBytes": 0,
  "reportPeriod": "Report Period value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365groupsactivitydetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 802

{
  "@odata.type": "#microsoft.graph.office365GroupsActivityDetail",
  "id": "eb807999-7999-eb80-9979-80eb997980eb",
  "reportRefreshDate": "Date",
  "groupId": "Group Id value",
  "groupDisplayName": "Group Display Name value",
  "isDeleted": true,
  "ownerPrincipalName": "Owner Principal Name value",
  "lastActivityDate": "Date",
  "groupType": "Group Type value",
  "memberCount": 11,
  "externalMemberCount": 3,
  "exchangeReceivedEmailCount": 10,
  "sharePointActiveFileCount": 9,
  "yammerPostedMessageCount": 8,
  "yammerReadMessageCount": 6,
  "yammerLikedMessageCount": 7,
  "exchangeMailboxTotalItemCount": 13,
  "exchangeMailboxStorageUsedInBytes": 1,
  "sharePointTotalFileCount": 8,
  "sharePointSiteStorageUsedInBytes": 0,
  "reportPeriod": "Report Period value"
}
```


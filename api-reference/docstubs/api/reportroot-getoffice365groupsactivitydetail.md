---
title: "reportRoot: getOffice365GroupsActivityDetail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getOffice365GroupsActivityDetail

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getOffice365GroupsActivityDetail
GET /print/reports/{reportRootId}/getOffice365GroupsActivityDetail
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitydetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityDetail(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365groupsactivitydetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365GroupsActivityDetail",
      "id": "4aaad39e-d39e-4aaa-9ed3-aa4a9ed3aa4a",
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
  ]
}
```


---
title: "List office365GroupsActivityDetails"
description: "List properties and relationships of the office365GroupsActivityDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List office365GroupsActivityDetails

List properties and relationships of the [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) objects.

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
GET ** Collection URI for microsoft.graph.office365GroupsActivityDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_office365groupsactivitydetail"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.office365GroupsActivityDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365groupsactivitydetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 919

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365GroupsActivityDetail",
      "id": "9b0c0da2-0da2-9b0c-a20d-0c9ba20d0c9b",
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


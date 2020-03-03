---
title: "Get office365GroupsActivityCounts"
description: "Read properties and relationships of the office365GroupsActivityCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get office365GroupsActivityCounts

Read properties and relationships of the [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object.

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
GET ** Entity URI for microsoft.graph.office365GroupsActivityCounts not found
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
If successful, this method returns a `200 OK` response code and [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_office365groupsactivitycounts"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.office365GroupsActivityCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 375

{
  "value": {
    "@odata.type": "#microsoft.graph.office365GroupsActivityCounts",
    "id": "a282b8b1-b8b1-a282-b1b8-82a2b1b882a2",
    "reportRefreshDate": "Date",
    "exchangeEmailsReceived": 6,
    "yammerMessagesPosted": 4,
    "yammerMessagesRead": 2,
    "yammerMessagesLiked": 3,
    "reportDate": "Date",
    "reportPeriod": "Report Period value"
  }
}
```


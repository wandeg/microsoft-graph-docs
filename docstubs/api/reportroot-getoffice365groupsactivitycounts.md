---
title: "getOffice365GroupsActivityCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOffice365GroupsActivityCounts

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
GET /reports/getOffice365GroupsActivityCounts
GET /print/reports/{reportRootId}/getOffice365GroupsActivityCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Property|Type|Description|
|:---|:---|:---|
|period|String||



## Response
If successful, this function returns a `200 OK` response code and a [office365GroupsActivityCounts](../resources/office365groupsactivitycounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivitycounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365groupsactivitycounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 407

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365GroupsActivityCounts",
      "id": "a3ae2d55-2d55-a3ae-552d-aea3552daea3",
      "reportRefreshDate": "Date",
      "exchangeEmailsReceived": 6,
      "yammerMessagesPosted": 4,
      "yammerMessagesRead": 2,
      "yammerMessagesLiked": 3,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```


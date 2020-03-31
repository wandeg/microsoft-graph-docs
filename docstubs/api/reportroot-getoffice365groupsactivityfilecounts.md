---
title: "getOffice365GroupsActivityFileCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOffice365GroupsActivityFileCounts

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
GET /reports/getOffice365GroupsActivityFileCounts
GET /print/reports/{reportRootId}/getOffice365GroupsActivityFileCounts
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
If successful, this function returns a `200 OK` response code and a [office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365groupsactivityfilecounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365GroupsActivityFileCounts",
      "id": "838794ac-94ac-8387-ac94-8783ac948783",
      "reportRefreshDate": "Date",
      "total": 5,
      "active": 6,
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```


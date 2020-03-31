---
title: "getOffice365ServicesUserCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getOffice365ServicesUserCounts

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
GET /reports/getOffice365ServicesUserCounts
GET /print/reports/{reportRootId}/getOffice365ServicesUserCounts
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
If successful, this function returns a `200 OK` response code and a [office365ServicesUserCounts](../resources/office365servicesusercounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365servicesusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
      "id": "2ca7285d-285d-2ca7-5d28-a72c5d28a72c",
      "reportRefreshDate": "Date",
      "exchangeActive": 14,
      "exchangeInactive": 0,
      "oneDriveActive": 14,
      "oneDriveInactive": 0,
      "sharePointActive": 0,
      "sharePointInactive": 2,
      "skypeForBusinessActive": 6,
      "skypeForBusinessInactive": 8,
      "yammerActive": 12,
      "yammerInactive": 14,
      "teamsActive": 11,
      "teamsInactive": 13,
      "office365Active": 15,
      "office365Inactive": 1,
      "reportPeriod": "Report Period value"
    }
  ]
}
```


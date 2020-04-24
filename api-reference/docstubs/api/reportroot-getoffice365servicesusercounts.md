---
title: "reportRoot: getOffice365ServicesUserCounts"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getOffice365ServicesUserCounts

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
GET /reports/getOffice365ServicesUserCounts
GET /print/reports/{reportRootId}/getOffice365ServicesUserCounts
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
If successful, this function returns a `200 OK` response code and a [office365ServicesUserCounts](../resources/office365servicesusercounts.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.office365servicesusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
      "id": "60c94336-4336-60c9-3643-c9603643c960",
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


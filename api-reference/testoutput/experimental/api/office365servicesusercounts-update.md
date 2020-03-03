---
title: "Update office365ServicesUserCounts"
description: "Update the properties of a office365ServicesUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update office365ServicesUserCounts

Update the properties of a [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.office365ServicesUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [office365ServicesUserCounts](../resources/office365ServicesUserCounts.md) object.

The following table shows the properties that are required when you create the [office365ServicesUserCounts](../resources/office365servicesusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|exchangeActive|Int64||
|exchangeInactive|Int64||
|oneDriveActive|Int64||
|oneDriveInactive|Int64||
|sharePointActive|Int64||
|sharePointInactive|Int64||
|skypeForBusinessActive|Int64||
|skypeForBusinessInactive|Int64||
|yammerActive|Int64||
|yammerInactive|Int64||
|teamsActive|Int64||
|teamsInactive|Int64||
|office365Active|Int64||
|office365Inactive|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_office365servicesusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.office365ServicesUserCounts not found
Content-type: application/json
Content-length: 512

{
  "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
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
Content-Length: 561

{
  "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
  "id": "618f6b62-6b62-618f-626b-8f61626b8f61",
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
```


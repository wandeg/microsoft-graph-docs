---
title: "Create office365ServicesUserCounts"
description: "Create a new office365ServicesUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create office365ServicesUserCounts

Namespace: microsoft.graph

Create a new [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.office365ServicesUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.

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
If successful, this method returns a `201 Created` response code and a [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_office365servicesusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.office365ServicesUserCounts not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.office365servicesusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 561

{
  "@odata.type": "#microsoft.graph.office365ServicesUserCounts",
  "id": "6c9949b7-49b7-6c99-b749-996cb749996c",
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


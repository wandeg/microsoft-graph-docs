---
title: "Get office365ServicesUserCounts"
description: "Read properties and relationships of the office365ServicesUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get office365ServicesUserCounts

Namespace: microsoft.graph

Read properties and relationships of the [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object.

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
GET ** Entity URI for microsoft.graph.office365ServicesUserCounts not found
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
If successful, this method returns a `200 OK` response code and [office365ServicesUserCounts](../resources/office365servicesusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_office365servicesusercounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.office365ServicesUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 616

{
  "value": {
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
}
```


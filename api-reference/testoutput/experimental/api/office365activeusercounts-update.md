---
title: "Update office365ActiveUserCounts"
description: "Update the properties of a office365ActiveUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update office365ActiveUserCounts

Namespace: microsoft.graph

Update the properties of a [office365ActiveUserCounts](../resources/office365activeusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.office365ActiveUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [office365ActiveUserCounts](../resources/office365activeusercounts.md) object.

The following table shows the properties that are required when you create the [office365ActiveUserCounts](../resources/office365activeusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|office365|Int64||
|exchange|Int64||
|oneDrive|Int64||
|sharePoint|Int64||
|skypeForBusiness|Int64||
|yammer|Int64||
|teams|Int64||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [office365ActiveUserCounts](../resources/office365activeusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_office365activeusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.office365ActiveUserCounts not found
Content-type: application/json
Content-length: 299

{
  "@odata.type": "#microsoft.graph.office365ActiveUserCounts",
  "reportRefreshDate": "Date",
  "office365": 9,
  "exchange": 8,
  "oneDrive": 8,
  "sharePoint": 10,
  "skypeForBusiness": 0,
  "yammer": 6,
  "teams": 5,
  "reportDate": "Date",
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
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.office365ActiveUserCounts",
  "id": "a346dbc0-dbc0-a346-c0db-46a3c0db46a3",
  "reportRefreshDate": "Date",
  "office365": 9,
  "exchange": 8,
  "oneDrive": 8,
  "sharePoint": 10,
  "skypeForBusiness": 0,
  "yammer": 6,
  "teams": 5,
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```


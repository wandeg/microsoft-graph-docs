---
title: "Update skypeForBusinessPeerToPeerActivityUserCounts"
description: "Update the properties of a skypeForBusinessPeerToPeerActivityUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update skypeForBusinessPeerToPeerActivityUserCounts

Update the properties of a [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) object.

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
PATCH ** Entity URI for microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeForBusinessPeerToPeerActivityUserCounts.md) object.

The following table shows the properties that are required when you create the [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|im|Int64||
|audio|Int64||
|video|Int64||
|appSharing|Int64||
|fileTransfer|Int64||
|reportRefreshDate|Date||
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [skypeForBusinessPeerToPeerActivityUserCounts](../resources/skypeforbusinesspeertopeeractivityusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_skypeforbusinesspeertopeeractivityusercounts"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts not found
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts",
  "im": 2,
  "audio": 5,
  "video": 5,
  "appSharing": 10,
  "fileTransfer": 12,
  "reportRefreshDate": "Date",
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
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityUserCounts",
  "id": "ecaada39-da39-ecaa-39da-aaec39daaaec",
  "im": 2,
  "audio": 5,
  "video": 5,
  "appSharing": 10,
  "fileTransfer": 12,
  "reportRefreshDate": "Date",
  "reportDate": "Date",
  "reportPeriod": "Report Period value"
}
```


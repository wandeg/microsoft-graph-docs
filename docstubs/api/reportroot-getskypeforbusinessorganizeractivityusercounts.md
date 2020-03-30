---
title: "getSkypeForBusinessOrganizerActivityUserCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getSkypeForBusinessOrganizerActivityUserCounts

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
GET /reports/getSkypeForBusinessOrganizerActivityUserCounts
GET /print/reports/{reportRootId}/getSkypeForBusinessOrganizerActivityUserCounts
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
If successful, this function returns a `200 OK` response code and a [skypeForBusinessOrganizerActivityUserCounts](../resources/skypeforbusinessorganizeractivityusercounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessorganizeractivityusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessOrganizerActivityUserCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.skypeforbusinessorganizeractivityusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 432

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.skypeForBusinessOrganizerActivityUserCounts",
      "id": "783a02b3-02b3-783a-b302-3a78b3023a78",
      "im": 2,
      "audioVideo": 10,
      "appSharing": 10,
      "web": 3,
      "dialInOut3rdParty": 1,
      "dialInOutMicrosoft": 2,
      "reportRefreshDate": "Date",
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```


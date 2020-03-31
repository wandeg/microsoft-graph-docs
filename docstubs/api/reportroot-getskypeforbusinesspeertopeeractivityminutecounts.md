---
title: "getSkypeForBusinessPeerToPeerActivityMinuteCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getSkypeForBusinessPeerToPeerActivityMinuteCounts

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
GET /reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts
GET /print/reports/{reportRootId}/getSkypeForBusinessPeerToPeerActivityMinuteCounts
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
If successful, this function returns a `200 OK` response code and a [skypeForBusinessPeerToPeerActivityMinuteCounts](../resources/skypeforbusinesspeertopeeractivityminutecounts.md) collection in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinesspeertopeeractivityminutecounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessPeerToPeerActivityMinuteCounts(period='parameterValue')
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.skypeforbusinesspeertopeeractivityminutecounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 327

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.skypeForBusinessPeerToPeerActivityMinuteCounts",
      "id": "d1e76d9b-6d9b-d1e7-9b6d-e7d19b6de7d1",
      "audio": 5,
      "video": 5,
      "reportRefreshDate": "Date",
      "reportDate": "Date",
      "reportPeriod": "Report Period value"
    }
  ]
}
```


---
title: "reportRoot: getEmailAppUsageVersionsUserCounts"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# getEmailAppUsageVersionsUserCounts

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
GET /reports/getEmailAppUsageVersionsUserCounts
GET /print/reports/{reportRootId}/getEmailAppUsageVersionsUserCounts
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
If successful, this function returns a `200 OK` response code and a [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageversionsusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageVersionsUserCounts(period='parameterValue')
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailappusageversionsusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 376

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
      "id": "5ac22113-2113-5ac2-1321-c25a1321c25a",
      "reportRefreshDate": "Date",
      "outlook2016": 11,
      "outlook2013": 11,
      "outlook2010": 11,
      "outlook2007": 11,
      "undetermined": 12,
      "reportPeriod": "Report Period value"
    }
  ]
}
```


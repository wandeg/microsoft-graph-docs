---
title: "List emailAppUsageAppsUserCountses"
description: "List properties and relationships of the emailAppUsageAppsUserCounts objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List emailAppUsageAppsUserCountses

List properties and relationships of the [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) objects.

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
GET ** Collection URI for microsoft.graph.emailAppUsageAppsUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailappusageappsusercounts"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.emailAppUsageAppsUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailappusageappsusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailAppUsageAppsUserCounts",
      "id": "29843b93-3b93-2984-933b-8429933b8429",
      "reportRefreshDate": "Date",
      "mailForMac": 10,
      "outlookForMac": 13,
      "outlookForWindows": 1,
      "outlookForMobile": 0,
      "otherForMobile": 14,
      "outlookForWeb": 13,
      "pop3App": 7,
      "imap4App": 8,
      "smtpApp": 7,
      "reportPeriod": "Report Period value"
    }
  ]
}
```


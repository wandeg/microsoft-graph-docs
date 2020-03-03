---
title: "Get emailAppUsageAppsUserCounts"
description: "Read properties and relationships of the emailAppUsageAppsUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get emailAppUsageAppsUserCounts

Namespace: microsoft.graph

Read properties and relationships of the [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) object.

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
GET ** Entity URI for microsoft.graph.emailAppUsageAppsUserCounts not found
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
If successful, this method returns a `200 OK` response code and [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailappusageappsusercounts"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.emailAppUsageAppsUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 436

{
  "value": {
    "@odata.type": "#microsoft.graph.emailAppUsageAppsUserCounts",
    "id": "7e4b278f-278f-7e4b-8f27-4b7e8f274b7e",
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
}
```


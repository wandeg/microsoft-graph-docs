---
title: "Get emailAppUsageUserCounts"
description: "Read properties and relationships of the emailAppUsageUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get emailAppUsageUserCounts

Read properties and relationships of the [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object.

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
GET ** Entity URI for microsoft.graph.emailAppUsageUserCounts not found
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
If successful, this method returns a `200 OK` response code and [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailappusageusercounts"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.emailAppUsageUserCounts not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 459

{
  "value": {
    "@odata.type": "#microsoft.graph.emailAppUsageUserCounts",
    "id": "b5dd91b8-91b8-b5dd-b891-ddb5b891ddb5",
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
    "reportDate": "Date",
    "reportPeriod": "Report Period value"
  }
}
```


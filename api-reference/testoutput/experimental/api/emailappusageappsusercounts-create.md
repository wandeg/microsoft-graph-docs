---
title: "Create emailAppUsageAppsUserCounts"
description: "Create a new emailAppUsageAppsUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create emailAppUsageAppsUserCounts

Create a new [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.emailAppUsageAppsUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the emailAppUsageAppsUserCounts object.

The following table shows the properties that are required when you create the emailAppUsageAppsUserCounts.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|mailForMac|Int64||
|outlookForMac|Int64||
|outlookForWindows|Int64||
|outlookForMobile|Int64||
|otherForMobile|Int64||
|outlookForWeb|Int64||
|pop3App|Int64||
|imap4App|Int64||
|smtpApp|Int64||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_emailappusageappsusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.emailAppUsageAppsUserCounts not found
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.emailAppUsageAppsUserCounts",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailappusageappsusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

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
```


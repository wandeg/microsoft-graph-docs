---
title: "Create emailAppUsageUserCounts"
description: "Create a new emailAppUsageUserCounts object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create emailAppUsageUserCounts

Namespace: microsoft.graph

Create a new [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.emailAppUsageUserCounts not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object.

The following table shows the properties that are required when you create the [emailAppUsageUserCounts](../resources/emailappusageusercounts.md).

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
|reportDate|Date||
|reportPeriod|String||



## Response
If successful, this method returns a `201 Created` response code and a [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_emailappusageusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.emailAppUsageUserCounts not found
Content-type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.emailAppUsageUserCounts",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailappusageusercounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 412

{
  "@odata.type": "#microsoft.graph.emailAppUsageUserCounts",
  "id": "282999f4-99f4-2829-f499-2928f4992928",
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
```


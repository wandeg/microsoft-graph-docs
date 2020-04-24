---
title: "reportRoot: getEmailAppUsageUserCounts"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getEmailAppUsageUserCounts

Namespace: microsoft.graph

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/getEmailAppUsageUserCounts
GET /print/reports/{reportRootId}/getEmailAppUsageUserCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailappusageusercounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailAppUsageUserCounts",
      "id": "781be35e-e35e-781b-5ee3-1b785ee31b78",
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
  ]
}
```


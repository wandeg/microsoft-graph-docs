---
title: "reportRoot: getEmailAppUsageUserDetail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getEmailAppUsageUserDetail

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
GET /reports/getEmailAppUsageUserDetail
GET /print/reports/{reportRootId}/getEmailAppUsageUserDetail
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
If successful, this function returns a `200 OK` response code and a [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='parameterValue')
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailappusageuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailAppUsageUserDetail",
      "id": "859a9acc-9acc-859a-cc9a-9a85cc9a9a85",
      "reportRefreshDate": "Date",
      "userPrincipalName": "User Principal Name value",
      "displayName": "Display Name value",
      "isDeleted": true,
      "deletedDate": "Date",
      "lastActivityDate": "Date",
      "mailForMac": [
        "Mail For Mac value"
      ],
      "outlookForMac": [
        "Outlook For Mac value"
      ],
      "outlookForWindows": [
        "Outlook For Windows value"
      ],
      "outlookForMobile": [
        "Outlook For Mobile value"
      ],
      "otherForMobile": [
        "Other For Mobile value"
      ],
      "outlookForWeb": [
        "Outlook For Web value"
      ],
      "pop3App": [
        "Pop3App value"
      ],
      "imap4App": [
        "Imap4App value"
      ],
      "smtpApp": [
        "Smtp App value"
      ],
      "reportPeriod": "Report Period value"
    }
  ]
}
```


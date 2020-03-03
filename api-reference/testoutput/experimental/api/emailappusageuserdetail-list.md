---
title: "List emailAppUsageUserDetails"
description: "List properties and relationships of the emailAppUsageUserDetail objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List emailAppUsageUserDetails

Namespace: microsoft.graph

List properties and relationships of the [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) objects.

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
GET ** Collection URI for microsoft.graph.emailAppUsageUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_emailappusageuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.emailAppUsageUserDetail not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.emailappusageuserdetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1021

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailAppUsageUserDetail",
      "id": "aba24636-4636-aba2-3646-a2ab3646a2ab",
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


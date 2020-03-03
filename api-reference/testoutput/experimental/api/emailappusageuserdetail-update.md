---
title: "Update emailAppUsageUserDetail"
description: "Update the properties of a emailAppUsageUserDetail object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update emailAppUsageUserDetail

Update the properties of a [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) object.

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
PATCH ** Entity URI for microsoft.graph.emailAppUsageUserDetail not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [emailAppUsageUserDetail](../resources/emailAppUsageUserDetail.md) object.

The following table shows the properties that are required when you create the [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportRefreshDate|Date||
|userPrincipalName|String||
|displayName|String||
|isDeleted|Boolean||
|deletedDate|Date||
|lastActivityDate|Date||
|mailForMac|String collection||
|outlookForMac|String collection||
|outlookForWindows|String collection||
|outlookForMobile|String collection||
|otherForMobile|String collection||
|outlookForWeb|String collection||
|pop3App|String collection||
|imap4App|String collection||
|smtpApp|String collection||
|reportPeriod|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_emailappusageuserdetail"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.emailAppUsageUserDetail not found
Content-type: application/json
Content-length: 795

{
  "@odata.type": "#microsoft.graph.emailAppUsageUserDetail",
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
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 844

{
  "@odata.type": "#microsoft.graph.emailAppUsageUserDetail",
  "id": "32a267ca-67ca-32a2-ca67-a232ca67a232",
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
```


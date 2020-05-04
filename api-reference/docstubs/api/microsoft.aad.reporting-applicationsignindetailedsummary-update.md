---
title: "Update applicationSignInDetailedSummary"
description: "Update the properties of a applicationSignInDetailedSummary object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update applicationSignInDetailedSummary

Namespace: Microsoft.AAD.Reporting

Update the properties of a [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object.

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
PATCH /reports/applicationSignInDetailedSummary/{applicationSignInDetailedSummaryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object.

The following table shows the properties that are required when you create the [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|appDisplayName|String|**TODO: Add Description**|
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)|**TODO: Add Description**|
|signInCount|Int64|**TODO: Add Description**|
|aggregatedEventDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_applicationsignindetailedsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{applicationSignInDetailedSummaryId}
Content-Type: application/json
Content-length: 447

{
  "@odata.type": "#Microsoft.AAD.Reporting.applicationSignInDetailedSummary",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "status": {
    "@odata.type": "Microsoft.AAD.Reporting.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "signInCount": 11,
  "aggregatedEventDateTime": "2016-12-31T23:59:43.9824644+03:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#Microsoft.AAD.Reporting.applicationSignInDetailedSummary",
  "id": "def9daf5-daf5-def9-f5da-f9def5daf9de",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "status": {
    "@odata.type": "Microsoft.AAD.Reporting.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "signInCount": 11,
  "aggregatedEventDateTime": "2016-12-31T23:59:43.9824644+03:00"
}
```


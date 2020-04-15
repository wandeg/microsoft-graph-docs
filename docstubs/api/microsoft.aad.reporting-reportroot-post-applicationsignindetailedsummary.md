---
title: "Add applicationSignInDetailedSummary"
description: "Add applicationSignInDetailedSummary by posting to the applicationSignInDetailedSummary collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add applicationSignInDetailedSummary

Namespace: Microsoft.AAD.Reporting

Add applicationSignInDetailedSummary by posting to the applicationSignInDetailedSummary collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /reports/applicationSignInDetailedSummary/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object.

The following table shows the properties that are required when you create the [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|appId|String||
|appDisplayName|String||
|status|[signInStatus](../resources/microsoft.aad.reporting-signinstatus.md)||
|signInCount|Int64||
|aggregatedEventDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_applicationsignindetailedsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary
Content-type: application/json
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
  "aggregatedEventDateTime": "2017-01-01T00:02:58.7292094+00:00"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.aad.reporting.applicationsignindetailedsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 496

{
  "@odata.type": "#Microsoft.AAD.Reporting.applicationSignInDetailedSummary",
  "id": "cd78981b-981b-cd78-1b98-78cd1b9878cd",
  "appId": "App Id value",
  "appDisplayName": "App Display Name value",
  "status": {
    "@odata.type": "Microsoft.AAD.Reporting.signInStatus",
    "errorCode": 9,
    "failureReason": "Failure Reason value",
    "additionalDetails": "Additional Details value"
  },
  "signInCount": 11,
  "aggregatedEventDateTime": "2017-01-01T00:02:58.7292094+00:00"
}
```


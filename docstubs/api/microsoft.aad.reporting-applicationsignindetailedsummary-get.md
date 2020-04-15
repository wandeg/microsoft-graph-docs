---
title: "Get applicationSignInDetailedSummary"
description: "Read properties and relationships of the applicationSignInDetailedSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get applicationSignInDetailedSummary

Namespace: Microsoft.AAD.Reporting

Read properties and relationships of the [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object.

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
GET /reports/applicationSignInDetailedSummary/{applicationSignInDetailedSummaryId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [applicationSignInDetailedSummary](../resources/microsoft.aad.reporting-applicationsignindetailedsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/{applicationSignInDetailedSummaryId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.applicationSignInDetailedSummary"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 539

{
  "value": {
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
}
```


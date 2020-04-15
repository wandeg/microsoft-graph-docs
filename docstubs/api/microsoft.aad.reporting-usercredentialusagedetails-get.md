---
title: "Get userCredentialUsageDetails"
description: "Read properties and relationships of the userCredentialUsageDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get userCredentialUsageDetails

Namespace: Microsoft.AAD.Reporting

Read properties and relationships of the [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object.

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
GET /reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
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
If successful, this method returns a `200 OK` response code and [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_usercredentialusagedetails"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.AAD.Reporting.userCredentialUsageDetails"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 438

{
  "value": {
    "@odata.type": "#Microsoft.AAD.Reporting.userCredentialUsageDetails",
    "id": "439daf1d-af1d-439d-1daf-9d431daf9d43",
    "feature": "String",
    "userPrincipalName": "User Principal Name value",
    "userDisplayName": "User Display Name value",
    "isSuccess": true,
    "authMethod": "String",
    "failureReason": "Failure Reason value",
    "eventDateTime": "2016-12-31T23:58:34.1704434+00:00"
  }
}
```


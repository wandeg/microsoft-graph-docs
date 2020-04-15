---
title: "Update userCredentialUsageDetails"
description: "Update the properties of a userCredentialUsageDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userCredentialUsageDetails

Namespace: Microsoft.AAD.Reporting

Update the properties of a [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object.

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
PATCH /reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object.

The following table shows the properties that are required when you create the [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String||
|feature|Enumeration| Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|userPrincipalName|String||
|userDisplayName|String||
|isSuccess|Boolean||
|authMethod|Enumeration| Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|failureReason|String||
|eventDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_usercredentialusagedetails"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
Content-type: application/json
Content-length: 352

{
  "@odata.type": "#Microsoft.AAD.Reporting.userCredentialUsageDetails",
  "feature": "String",
  "userPrincipalName": "User Principal Name value",
  "userDisplayName": "User Display Name value",
  "isSuccess": true,
  "authMethod": "String",
  "failureReason": "Failure Reason value",
  "eventDateTime": "2016-12-31T23:58:34.1704434+00:00"
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
Content-Length: 401

{
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
```


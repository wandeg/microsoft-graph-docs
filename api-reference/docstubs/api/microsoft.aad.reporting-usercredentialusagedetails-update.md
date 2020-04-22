---
title: "Update userCredentialUsageDetails"
description: "Update the properties of a userCredentialUsageDetails object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update userCredentialUsageDetails

Namespace: Microsoft.AAD.Reporting

Update the properties of a [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object.

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
PATCH /reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md) object.

The following table shows the properties that are required when you create the [userCredentialUsageDetails](../resources/microsoft.aad.reporting-usercredentialusagedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|feature|featureType|**TODO: Add Description**. Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|userPrincipalName|String|**TODO: Add Description**|
|userDisplayName|String|**TODO: Add Description**|
|isSuccess|Boolean|**TODO: Add Description**|
|authMethod|usageAuthMethod|**TODO: Add Description**. Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|failureReason|String|**TODO: Add Description**|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|



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
Content-Type: application/json
Content-length: 352

{
  "@odata.type": "#Microsoft.AAD.Reporting.userCredentialUsageDetails",
  "feature": "String",
  "userPrincipalName": "User Principal Name value",
  "userDisplayName": "User Display Name value",
  "isSuccess": true,
  "authMethod": "String",
  "failureReason": "Failure Reason value",
  "eventDateTime": "2017-01-01T00:00:09.6489218+00:00"
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
  "@odata.type": "#Microsoft.AAD.Reporting.userCredentialUsageDetails",
  "id": "a77cb125-b125-a77c-25b1-7ca725b17ca7",
  "feature": "String",
  "userPrincipalName": "User Principal Name value",
  "userDisplayName": "User Display Name value",
  "isSuccess": true,
  "authMethod": "String",
  "failureReason": "Failure Reason value",
  "eventDateTime": "2017-01-01T00:00:09.6489218+00:00"
}
```


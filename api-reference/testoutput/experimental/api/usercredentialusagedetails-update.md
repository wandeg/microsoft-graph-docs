---
title: "Update userCredentialUsageDetails"
description: "Update the properties of a userCredentialUsageDetails object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update userCredentialUsageDetails

Namespace: microsoft.graph

Update the properties of a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.

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
PATCH /reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.

The following table shows the properties that are required when you create the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|feature|Enumeration|. Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|userPrincipalName|String||
|userDisplayName|String||
|isSuccess|Boolean||
|authMethod|Enumeration|. Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|failureReason|String||
|eventDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_usercredentialusagedetails"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/reports/userCredentialUsageDetails/{userCredentialUsageDetailsId}
Content-type: application/json
Content-length: 344

{
  "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
  "feature": "String",
  "userPrincipalName": "User Principal Name value",
  "userDisplayName": "User Display Name value",
  "isSuccess": true,
  "authMethod": "String",
  "failureReason": "Failure Reason value",
  "eventDateTime": "2017-01-01T00:01:42.7768776+03:00"
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
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
  "id": "149bdb35-db35-149b-35db-9b1435db9b14",
  "feature": "String",
  "userPrincipalName": "User Principal Name value",
  "userDisplayName": "User Display Name value",
  "isSuccess": true,
  "authMethod": "String",
  "failureReason": "Failure Reason value",
  "eventDateTime": "2017-01-01T00:01:42.7768776+03:00"
}
```


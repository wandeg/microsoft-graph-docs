---
title: "Add userCredentialUsageDetails"
description: "Add userCredentialUsageDetails by posting to the userCredentialUsageDetails collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add userCredentialUsageDetails

Namespace: microsoft.graph

Add userCredentialUsageDetails by posting to the userCredentialUsageDetails collection.

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
POST /reports/userCredentialUsageDetails/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object.

The following table shows the properties that are required when you create the [userCredentialUsageDetails](../resources/usercredentialusagedetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|feature|Enumeration| Possible values are: `registration`, `reset`, `unknownFutureValue`.|
|userPrincipalName|String||
|userDisplayName|String||
|isSuccess|Boolean||
|authMethod|Enumeration| Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion`, `appNotification`, `appCode`, `alternateMobileCall`, `fido`, `appPassword`, `unknownFutureValue`.|
|failureReason|String||
|eventDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [userCredentialUsageDetails](../resources/usercredentialusagedetails.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_usercredentialusagedetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/reports/userCredentialUsageDetails
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
  "eventDateTime": "2016-12-31T23:59:13.0497597+00:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.usercredentialusagedetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 393

{
  "@odata.type": "#microsoft.graph.userCredentialUsageDetails",
  "id": "5c5e076d-076d-5c5e-6d07-5e5c6d075e5c",
  "feature": "String",
  "userPrincipalName": "User Principal Name value",
  "userDisplayName": "User Display Name value",
  "isSuccess": true,
  "authMethod": "String",
  "failureReason": "Failure Reason value",
  "eventDateTime": "2016-12-31T23:59:13.0497597+00:00"
}
```


---
title: "Get advancedThreatProtectionOnboardingDeviceSettingState"
description: "Read the properties and relationships of an advancedThreatProtectionOnboardingDeviceSettingState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get advancedThreatProtectionOnboardingDeviceSettingState

Namespace: microsoft.graph

Read the properties and relationships of an [advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) object.

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
GET /deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and an [advancedThreatProtectionOnboardingDeviceSettingState](../resources/advancedthreatprotectiononboardingdevicesettingstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_advancedthreatprotectiononboardingdevicesettingstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/advancedThreatProtectionOnboardingStateSummary/advancedThreatProtectionOnboardingDeviceSettingStates/{advancedThreatProtectionOnboardingDeviceSettingStateId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.advancedThreatProtectionOnboardingDeviceSettingState",
    "id": "9559a07b-a07b-9559-7ba0-59957ba05995",
    "platformType": "String",
    "setting": "String",
    "settingName": "String",
    "deviceId": "String",
    "deviceName": "String",
    "userId": "String",
    "userEmail": "String",
    "userName": "String",
    "userPrincipalName": "String",
    "deviceModel": "String",
    "state": "String",
    "complianceGracePeriodExpirationDateTime": "String (timestamp)"
  }
}
```


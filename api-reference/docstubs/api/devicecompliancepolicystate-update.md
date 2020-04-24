---
title: "Update deviceCompliancePolicyState"
description: "Update the properties of a deviceCompliancePolicyState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceCompliancePolicyState

Namespace: microsoft.graph

Update the properties of a [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.

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
PATCH /invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingStates|[deviceCompliancePolicySettingState](../resources/devicecompliancepolicysettingstate.md) collection|**TODO: Add Description**|
|displayName|String|The name of the policy for this policyBase|
|version|Int32|The version of the policy|
|platformType|policyPlatformType|Platform type that the policy applies to. Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `windows10XProfile`, `all`.|
|state|complianceStatus|The compliance state of the policy. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|settingCount|Int32|Count of how many setting a policy holds|
|userId|String|User unique identifier, must be Guid|
|userPrincipalName|String|User Principal Name|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceCompliancePolicyState](../resources/devicecompliancepolicystate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicecompliancepolicystate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/managedDevices/{managedDeviceId}/deviceCompliancePolicyStates/{deviceCompliancePolicyStateId}
Content-Type: application/json
Content-length: 1102

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "String",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value",
      "settingInstanceId": "Setting Instance Id value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "String",
  "state": "String",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyState",
  "id": "034b0749-0749-034b-4907-4b0349074b03",
  "settingStates": [
    {
      "@odata.type": "microsoft.graph.deviceCompliancePolicySettingState",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "instanceDisplayName": "Instance Display Name value",
      "state": "String",
      "errorCode": 9,
      "errorDescription": "Error Description value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userEmail": "User Email value",
      "userPrincipalName": "User Principal Name value",
      "sources": [
        {
          "@odata.type": "microsoft.graph.settingSource",
          "id": "Id value",
          "displayName": "Display Name value"
        }
      ],
      "currentValue": "Current Value value",
      "settingInstanceId": "Setting Instance Id value"
    }
  ],
  "displayName": "Display Name value",
  "version": 7,
  "platformType": "String",
  "state": "String",
  "settingCount": 12,
  "userId": "User Id value",
  "userPrincipalName": "User Principal Name value"
}
```


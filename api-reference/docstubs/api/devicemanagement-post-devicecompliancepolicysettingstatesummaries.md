---
title: "Create deviceCompliancePolicySettingStateSummaries"
description: "Create a new deviceCompliancePolicySettingStateSummaries object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceCompliancePolicySettingStateSummaries

Namespace: microsoft.graph

Create a new deviceCompliancePolicySettingStateSummaries object.

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
POST /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object.

The following table shows the properties that are required when you create the [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|setting|String|The setting class name and property name.|
|settingName|String|Name of the setting.|
|platformType|policyPlatformType|Setting platform. Possible values are: `android`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `all`.|
|unknownDeviceCount|Int32|Number of unknown devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|compliantDeviceCount|Int32|Number of compliant devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|errorDeviceCount|Int32|Number of error devices|
|conflictDeviceCount|Int32|Number of conflict devices|



## Response
If successful, this method returns a `201 Created` response code and a [deviceCompliancePolicySettingStateSummary](../resources/devicecompliancepolicysettingstatesummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancepolicysettingstatesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
Content-Type: application/json
Content-length: 394

{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "String",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicecompliancepolicysettingstatesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
  "id": "4ec1130a-130a-4ec1-0a13-c14e0a13c14e",
  "setting": "Setting value",
  "settingName": "Setting Name value",
  "platformType": "String",
  "unknownDeviceCount": 2,
  "notApplicableDeviceCount": 8,
  "compliantDeviceCount": 4,
  "remediatedDeviceCount": 5,
  "nonCompliantDeviceCount": 7,
  "errorDeviceCount": 0,
  "conflictDeviceCount": 3
}
```


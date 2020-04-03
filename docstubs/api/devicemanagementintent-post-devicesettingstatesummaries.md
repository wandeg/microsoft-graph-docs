---
title: "Add deviceSettingStateSummaries"
description: "Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceSettingStateSummaries

Namespace: microsoft.graph

Add deviceSettingStateSummaries by posting to the deviceSettingStateSummaries collection.

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
POST /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|settingName|String||
|compliantCount|Int32||
|conflictCount|Int32||
|errorCount|Int32||
|nonCompliantCount|Int32||
|notApplicableCount|Int32||
|remediatedCount|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementintentdevicesettingstatesummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
Content-type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementintentdevicesettingstatesummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 329

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "153ab0d2-b0d2-153a-d2b0-3a15d2b03a15",
  "settingName": "Setting Name value",
  "compliantCount": 14,
  "conflictCount": 13,
  "errorCount": 10,
  "nonCompliantCount": 1,
  "notApplicableCount": 2,
  "remediatedCount": 15
}
```


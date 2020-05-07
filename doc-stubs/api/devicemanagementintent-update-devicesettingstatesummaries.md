---
title: "Update deviceSettingStateSummaries"
description: "Update the properties of a deviceSettingStateSummaries object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceSettingStateSummaries

Namespace: microsoft.graph

Update the properties of a deviceSettingStateSummaries object.

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
PATCH /deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|settingName|String|**TODO: Add Description**|
|compliantCount|Int32|**TODO: Add Description**|
|conflictCount|Int32|**TODO: Add Description**|
|errorCount|Int32|**TODO: Add Description**|
|nonCompliantCount|Int32|**TODO: Add Description**|
|notApplicableCount|Int32|**TODO: Add Description**|
|remediatedCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentDeviceSettingStateSummary](../resources/devicemanagementintentdevicesettingstatesummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicesettingstatesummaries"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/deviceSettingStateSummaries
Content-Type: application/json
Content-length: 312

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "settingName": "String",
  "compliantCount": "Integer",
  "conflictCount": "Integer",
  "errorCount": "Integer",
  "nonCompliantCount": "Integer",
  "notApplicableCount": "Integer",
  "remediatedCount": "Integer"
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
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceSettingStateSummary",
  "id": "5cdf7a38-7a38-5cdf-387a-df5c387adf5c",
  "settingName": "String",
  "compliantCount": "Integer",
  "conflictCount": "Integer",
  "errorCount": "Integer",
  "nonCompliantCount": "Integer",
  "notApplicableCount": "Integer",
  "remediatedCount": "Integer"
}
```


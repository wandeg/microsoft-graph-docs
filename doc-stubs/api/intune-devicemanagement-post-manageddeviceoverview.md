---
title: "Add managedDeviceOverview"
description: "Add managedDeviceOverview by posting to the managedDeviceOverview collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add managedDeviceOverview

Namespace: microsoft.graph

Add managedDeviceOverview by posting to the managedDeviceOverview collection.

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
POST /deviceManagement/managedDeviceOverview/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDeviceOverview](../resources/intune-manageddeviceoverview.md) object.

The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/intune-manageddeviceoverview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|enrolledDeviceCount|Int32|**TODO: Add Description**|
|mdmEnrolledCount|Int32|**TODO: Add Description**|
|dualEnrolledDeviceCount|Int32|**TODO: Add Description**|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/intune-deviceoperatingsystemsummary.md)|**TODO: Add Description**|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/intune-deviceexchangeaccessstatesummary.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [managedDeviceOverview](../resources/intune-manageddeviceoverview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_manageddeviceoverview_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/managedDeviceOverview/$ref
Content-Type: application/json
Content-length: 403

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "enrolledDeviceCount": "Integer",
  "mdmEnrolledCount": "Integer",
  "dualEnrolledDeviceCount": "Integer",
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
  }
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.manageddeviceoverview"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "id": "741b145f-145f-741b-5f14-1b745f141b74",
  "enrolledDeviceCount": "Integer",
  "mdmEnrolledCount": "Integer",
  "dualEnrolledDeviceCount": "Integer",
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.graph.deviceOperatingSystemSummary"
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.graph.deviceExchangeAccessStateSummary"
  }
}
```


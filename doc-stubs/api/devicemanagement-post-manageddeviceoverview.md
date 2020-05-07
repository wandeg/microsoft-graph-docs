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
In the request body, supply a JSON representation of the [managedDeviceOverview](../resources/manageddeviceoverview.md) object.

The following table shows the properties that are required when you create the [managedDeviceOverview](../resources/manageddeviceoverview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|Unique Identifier for the summary|
|enrolledDeviceCount|Int32|Total enrolled device count. Does not include PC devices managed via Intune PC Agent|
|mdmEnrolledCount|Int32|The number of devices enrolled in MDM|
|dualEnrolledDeviceCount|Int32|The number of devices enrolled in both MDM and EAS|
|deviceOperatingSystemSummary|[deviceOperatingSystemSummary](../resources/deviceoperatingsystemsummary.md)|Device operating system summary.|
|deviceExchangeAccessStateSummary|[deviceExchangeAccessStateSummary](../resources/deviceexchangeaccessstatesummary.md)|Distribution of Exchange Access State in Intune|
|managedDeviceModelsAndManufacturers|[managedDeviceModelsAndManufacturers](../resources/manageddevicemodelsandmanufacturers.md)|Models and Manufactures meatadata for managed devices in the account|
|lastModifiedDateTime|DateTimeOffset|Last modified date time of device overview|



## Response

If successful, this method returns a `204 No Content` response code and a [managedDeviceOverview](../resources/manageddeviceoverview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_manageddeviceoverview_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceOverview/$ref
Content-Type: application/json
Content-length: 599

{
  "@odata.type": "#microsoft.management.services.api.managedDeviceOverview",
  "enrolledDeviceCount": "Integer",
  "mdmEnrolledCount": "Integer",
  "dualEnrolledDeviceCount": "Integer",
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.management.services.api.deviceOperatingSystemSummary"
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.management.services.api.deviceExchangeAccessStateSummary"
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.management.services.api.managedDeviceModelsAndManufacturers"
  }
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.manageddeviceoverview"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.management.services.api.managedDeviceOverview",
  "id": "cddd2a41-2a41-cddd-412a-ddcd412addcd",
  "enrolledDeviceCount": "Integer",
  "mdmEnrolledCount": "Integer",
  "dualEnrolledDeviceCount": "Integer",
  "deviceOperatingSystemSummary": {
    "@odata.type": "microsoft.management.services.api.deviceOperatingSystemSummary"
  },
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "microsoft.management.services.api.deviceExchangeAccessStateSummary"
  },
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "microsoft.management.services.api.managedDeviceModelsAndManufacturers"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```


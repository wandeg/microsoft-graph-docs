---
title: "Update managedDeviceOverview"
description: ""
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: "microsoft-identity-platform"
doc_type: "apiPageType"
---

# Update managedDeviceOverview

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a managedDeviceOverview object.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from most to least privileged) |
| :------------------------------------- | :------------------------------------------ |
| Delegated (work or school account)     |                                             |
| Delegated (personal Microsoft account) |                                             |
| Application                            |                                             |

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

```http

```

## Request headers

| Name          | Description                 |
| :------------ | :-------------------------- |
| Authorization | Bearer {token}. Required.   |
| Content-Type  | application/json. Required. |

## Request body

In the request body, supply JSON representation of the managedDeviceOverview object.

The following table shows the properties that are required when you create the managedDeviceOverview object.

| Property                | Type                           | Description                           |
| :---------------------- | :----------------------------- | :------------------------------------ |
| $(this.Properties.Name) | $(this.Properties.DisplayType) | $(this.Properties.DisplayDescription) |

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [managedDeviceOverview](../resources/managedDeviceOverview.md) object in the response body.

## Examples

### Request

<!-- {
  "blockType": "request",
  "name": "update_manageddeviceoverview"
}
-->

```http
PATCH https://graph.microsoft.com/beta/

Content-Type: application/json
Content-Length: 1289

{
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": "Int32",
    "blockedDeviceCount": "Int32",
    "quarantinedDeviceCount": "Int32",
    "unavailableDeviceCount": "Int32",
    "unknownDeviceCount": "Int32"
  },
  "deviceOperatingSystemSummary": {
    "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
    "androidCorporateWorkProfileCount": "Int32",
    "androidCount": "Int32",
    "androidDedicatedCount": "Int32",
    "androidDeviceAdminCount": "Int32",
    "androidFullyManagedCount": "Int32",
    "androidWorkProfileCount": "Int32",
    "configMgrDeviceCount": "Int32",
    "iosCount": "Int32",
    "macOSCount": "Int32",
    "unknownCount": "Int32",
    "windowsCount": "Int32",
    "windowsMobileCount": "Int32"
  },
  "dualEnrolledDeviceCount": "Int32",
  "enrolledDeviceCount": "Int32",
  "lastModifiedDateTime": "DateTimeOffset",
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceManufacturers": [
      "String"
    ],
    "deviceModels": [
      "String"
    ]
  },
  "mdmEnrolledCount": "Int32"
}

```

### Response

**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.managedDeviceOverview"
}
-->

```http
HTTP 1.1 200 OK

Content-Type: application/json
{
  "value": {
  "@odata.type": "#microsoft.graph.managedDeviceOverview",
  "deviceExchangeAccessStateSummary": {
    "@odata.type": "#microsoft.graph.deviceExchangeAccessStateSummary",
    "allowedDeviceCount": "Int32",
    "blockedDeviceCount": "Int32",
    "quarantinedDeviceCount": "Int32",
    "unavailableDeviceCount": "Int32",
    "unknownDeviceCount": "Int32"
  },
  "deviceOperatingSystemSummary": {
    "@odata.type": "#microsoft.graph.deviceOperatingSystemSummary",
    "androidCorporateWorkProfileCount": "Int32",
    "androidCount": "Int32",
    "androidDedicatedCount": "Int32",
    "androidDeviceAdminCount": "Int32",
    "androidFullyManagedCount": "Int32",
    "androidWorkProfileCount": "Int32",
    "configMgrDeviceCount": "Int32",
    "iosCount": "Int32",
    "macOSCount": "Int32",
    "unknownCount": "Int32",
    "windowsCount": "Int32",
    "windowsMobileCount": "Int32"
  },
  "dualEnrolledDeviceCount": "Int32",
  "enrolledDeviceCount": "Int32",
  "id": "String(identifier)",
  "lastModifiedDateTime": "DateTimeOffset",
  "managedDeviceModelsAndManufacturers": {
    "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
    "deviceManufacturers": [
      "String"
    ],
    "deviceModels": [
      "String"
    ]
  },
  "mdmEnrolledCount": "Int32"
}
}

```
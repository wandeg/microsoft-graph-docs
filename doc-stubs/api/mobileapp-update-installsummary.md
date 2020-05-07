---
title: "Update installSummary"
description: "Update the properties of an installSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update installSummary

Namespace: microsoft.graph

Update the properties of an installSummary object.

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
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/installSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object.

The following table shows the properties that are required when you create the [mobileAppInstallSummary](../resources/mobileappinstallsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|**TODO: Add Description**|
|failedDeviceCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|notInstalledDeviceCount|Int32|**TODO: Add Description**|
|pendingInstallDeviceCount|Int32|**TODO: Add Description**|
|installedUserCount|Int32|**TODO: Add Description**|
|failedUserCount|Int32|**TODO: Add Description**|
|notApplicableUserCount|Int32|**TODO: Add Description**|
|notInstalledUserCount|Int32|**TODO: Add Description**|
|pendingInstallUserCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [mobileAppInstallSummary](../resources/mobileappinstallsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_installsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/installSummary
Content-Type: application/json
Content-length: 453

{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer",
  "pendingInstallDeviceCount": "Integer",
  "installedUserCount": "Integer",
  "failedUserCount": "Integer",
  "notApplicableUserCount": "Integer",
  "notInstalledUserCount": "Integer",
  "pendingInstallUserCount": "Integer"
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
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "13850852-0852-1385-5208-851352088513",
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer",
  "pendingInstallDeviceCount": "Integer",
  "installedUserCount": "Integer",
  "failedUserCount": "Integer",
  "notApplicableUserCount": "Integer",
  "notInstalledUserCount": "Integer",
  "pendingInstallUserCount": "Integer"
}
```


---
title: "Update userStatuses"
description: "Update the properties of a userStatuses object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userStatuses

Namespace: microsoft.graph

Update the properties of a userStatuses object.

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
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userAppInstallStatus](../resources/userappinstallstatus.md) object.

The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/userappinstallstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userName|String|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|installedDeviceCount|Int32|**TODO: Add Description**|
|failedDeviceCount|Int32|**TODO: Add Description**|
|notInstalledDeviceCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/userappinstallstatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userstatuses"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
Content-Type: application/json
Content-length: 235

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer"
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
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "35f695c4-95c4-35f6-c495-f635c495f635",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": "Integer",
  "failedDeviceCount": "Integer",
  "notInstalledDeviceCount": "Integer"
}
```


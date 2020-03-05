---
title: "Create eBookInstallSummary"
description: "Create a new eBookInstallSummary object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create eBookInstallSummary

Namespace: microsoft.graph

Create a new [eBookInstallSummary](../resources/ebookinstallsummary.md) object.

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
POST ** Collection URI for microsoft.graph.eBookInstallSummary not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/ebookinstallsummary.md) object.

The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/ebookinstallsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|installedDeviceCount|Int32|Number of Devices that have successfully installed this book.|
|failedDeviceCount|Int32|Number of Devices that have failed to install this book.|
|notInstalledDeviceCount|Int32|Number of Devices that does not have this book installed.|
|installedUserCount|Int32|Number of Users whose devices have all succeeded to install this book.|
|failedUserCount|Int32|Number of Users that have 1 or more device that failed to install this book.|
|notInstalledUserCount|Int32|Number of Users that did not install this book.|



## Response
If successful, this method returns a `201 Created` response code and a [eBookInstallSummary](../resources/ebookinstallsummary.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_ebookinstallsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.eBookInstallSummary not found
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ebookinstallsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "c168454f-454f-c168-4f45-68c14f4568c1",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```


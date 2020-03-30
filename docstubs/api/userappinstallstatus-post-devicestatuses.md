---
title: "Add deviceStatuses"
description: "Add deviceStatuses by posting to the deviceStatuses collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceStatuses

Namespace: microsoft.graph

Add deviceStatuses by posting to the deviceStatuses collection.

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
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object.

The following table shows the properties that are required when you create the [mobileAppInstallStatus](../resources/mobileappinstallstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceName|String||
|deviceId|String||
|lastSyncDateTime|DateTimeOffset||
|mobileAppInstallStatusValue|Enumeration| Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installState|Enumeration| Possible values are: `installed`, `failed`, `notInstalled`, `uninstallFailed`, `pendingInstall`, `unknown`, `notApplicable`.|
|installStateDetail|Enumeration| Possible values are: `noAdditionalDetails`, `dependencyFailedToInstall`, `dependencyWithRequirementsNotMet`, `dependencyPendingReboot`, `dependencyWithAutoInstallDisabled`, `seeInstallErrorCode`, `autoInstallDisabled`, `seeUninstallErrorCode`, `pendingReboot`, `installingDependencies`, `contentDownloaded`, `powerShellScriptRequirementNotMet`, `registryRequirementNotMet`, `fileSystemRequirementNotMet`, `platformNotApplicable`, `minimumCpuSpeedNotMet`, `minimumLogicalProcessorCountNotMet`, `minimumPhysicalMemoryNotMet`, `minimumOsVersionNotMet`, `minimumDiskSpaceNotMet`, `processorArchitectureNotApplicable`.|
|errorCode|Int32||
|osVersion|String||
|osDescription|String||
|userName|String||
|userPrincipalName|String||
|displayVersion|String||



## Response
If successful, this method returns a `201 Created` response code and a [mobileAppInstallStatus](../resources/mobileappinstallstatus.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_mobileappinstallstatus_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/deviceStatuses
Content-type: application/json
Content-length: 536

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2016-12-31T23:56:30.9655764+03:00",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mobileappinstallstatus"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.mobileAppInstallStatus",
  "id": "5e99ed89-ed89-5e99-89ed-995e89ed995e",
  "deviceName": "Device Name value",
  "deviceId": "Device Id value",
  "lastSyncDateTime": "2016-12-31T23:56:30.9655764+03:00",
  "mobileAppInstallStatusValue": "String",
  "installState": "String",
  "installStateDetail": "String",
  "errorCode": 9,
  "osVersion": "Os Version value",
  "osDescription": "Os Description value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "displayVersion": "Display Version value"
}
```


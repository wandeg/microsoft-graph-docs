---
title: "Add remoteActionAudits"
description: "Add remoteActionAudits by posting to the remoteActionAudits collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add remoteActionAudits

Namespace: microsoft.graph

Add remoteActionAudits by posting to the remoteActionAudits collection.

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
POST /deviceManagement/remoteActionAudits/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [remoteActionAudit](../resources/remoteactionaudit.md) object.

The following table shows the properties that are required when you create the [remoteActionAudit](../resources/remoteactionaudit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|deviceDisplayName|String||
|userName|String||
|initiatedByUserPrincipalName|String||
|action|Enumeration| Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.|
|requestDateTime|DateTimeOffset||
|deviceOwnerUserPrincipalName|String||
|deviceIMEI|String||
|actionState|Enumeration| Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|managedDeviceId|String||



## Response
If successful, this method returns a `201 Created` response code and a [remoteActionAudit](../resources/remoteactionaudit.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_remoteactionaudit_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "String",
  "requestDateTime": "2016-12-31T23:59:31.6365365+03:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "String",
  "managedDeviceId": "Managed Device Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.remoteactionaudit"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "2d721be2-1be2-2d72-e21b-722de21b722d",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "String",
  "requestDateTime": "2016-12-31T23:59:31.6365365+03:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "String",
  "managedDeviceId": "Managed Device Id value"
}
```


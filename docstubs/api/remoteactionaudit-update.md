---
title: "Update remoteActionAudit"
description: "Update the properties of a remoteActionAudit object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update remoteActionAudit

Namespace: microsoft.graph

Update the properties of a [remoteActionAudit](../resources/remoteactionaudit.md) object.

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
PATCH /deviceManagement/remoteActionAudits/{remoteActionAuditId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

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
If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/remoteactionaudit.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_remoteactionaudit"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits/{remoteActionAuditId}
Content-type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "String",
  "requestDateTime": "2016-12-31T23:59:14.9772779+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 546

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "4015e579-e579-4015-79e5-154079e51540",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "String",
  "requestDateTime": "2016-12-31T23:59:14.9772779+03:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "String",
  "managedDeviceId": "Managed Device Id value"
}
```


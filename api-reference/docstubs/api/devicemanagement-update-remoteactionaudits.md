---
title: "Update remoteActionAudits"
description: "Update the properties of a remoteActionAudits object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update remoteActionAudits

Namespace: microsoft.graph

Update the properties of a remoteActionAudits object.

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
PATCH /deviceManagement/remoteActionAudits
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [remoteActionAudit](../resources/remoteactionaudit.md) object.

The following table shows the properties that are required when you create the [remoteActionAudit](../resources/remoteactionaudit.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceDisplayName|String|Intune device name.|
|userName|String|\[deprecated\] Please use InitiatedByUserPrincipalName instead.|
|initiatedByUserPrincipalName|String|User who initiated the device action, format is UPN.|
|action|remoteAction|The action name. Possible values are: `unknown`, `factoryReset`, `removeCompanyData`, `resetPasscode`, `remoteLock`, `enableLostMode`, `disableLostMode`, `locateDevice`, `rebootNow`, `recoverPasscode`, `cleanWindowsDevice`, `logoutSharedAppleDeviceActiveUser`, `quickScan`, `fullScan`, `windowsDefenderUpdateSignatures`, `factoryResetKeepEnrollmentData`, `updateDeviceAccount`, `automaticRedeployment`, `shutDown`, `rotateBitLockerKeys`, `rotateFileVaultKey`, `getFileVaultKey`, `setDeviceName`.|
|requestDateTime|DateTimeOffset|Time when the action was issued, given in UTC.|
|deviceOwnerUserPrincipalName|String|Upn of the device owner.|
|deviceIMEI|String|IMEI of the device.|
|actionState|actionState|Action state. Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|managedDeviceId|String|Action target.|



## Response
If successful, this method returns a `200 OK` response code and an updated [remoteActionAudit](../resources/remoteactionaudit.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_remoteactionaudits"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/remoteActionAudits
Content-Type: application/json
Content-length: 497

{
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "String",
  "requestDateTime": "2017-01-01T00:02:26.8557697+03:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "String",
  "managedDeviceId": "Managed Device Id value"
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
  "@odata.type": "#microsoft.graph.remoteActionAudit",
  "id": "ee2db833-b833-ee2d-33b8-2dee33b82dee",
  "deviceDisplayName": "Device Display Name value",
  "userName": "User Name value",
  "initiatedByUserPrincipalName": "Initiated By User Principal Name value",
  "action": "String",
  "requestDateTime": "2017-01-01T00:02:26.8557697+03:00",
  "deviceOwnerUserPrincipalName": "Device Owner User Principal Name value",
  "deviceIMEI": "Device IMEI value",
  "actionState": "String",
  "managedDeviceId": "Managed Device Id value"
}
```


---
title: "Update deviceHealthScript"
description: "Update the properties of a deviceHealthScript object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceHealthScript

Namespace: microsoft.graph

Update the properties of a [deviceHealthScript](../resources/devicehealthscript.md) object.

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
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceHealthScript](../resources/devicehealthscript.md) object.

The following table shows the properties that are required when you create the [deviceHealthScript](../resources/devicehealthscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|publisher|String|Name of the device health script publisher|
|version|String|Version of the device health script|
|displayName|String|Name of the device health script|
|description|String|Description of the device health script|
|detectionScriptContent|Binary|The entire content of the detection powershell script|
|remediationScriptContent|Binary|The entire content of the remediation powershell script|
|createdDateTime|DateTimeOffset|The timestamp of when the device health script was created. This property is read-only.|
|lastModifiedDateTime|DateTimeOffset|The timestamp of when the device health script was modified. This property is read-only.|
|runAsAccount|runAsAccountType|Indicates the type of execution context. Possible values are: `system`, `user`.|
|enforceSignatureCheck|Boolean|Indicate whether the script signature needs be checked|
|runAs32Bit|Boolean|Indicate whether PowerShell script(s) should run as 32-bit|
|roleScopeTagIds|String collection|List of Scope Tag IDs for the device health script|
|isGlobalScript|Boolean|Determines if this is Microsoft Proprietary Script. Proprietary scripts are read-only|
|highestAvailableVersion|String|Highest available version for a Microsoft Proprietary script|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceHealthScript](../resources/devicehealthscript.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicehealthscript"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}
Content-Type: application/json
Content-length: 577

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
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
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "8fe3e3c4-e3c4-8fe3-c4e3-e38fc4e3e38f",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "isGlobalScript": true,
  "highestAvailableVersion": "Highest Available Version value"
}
```


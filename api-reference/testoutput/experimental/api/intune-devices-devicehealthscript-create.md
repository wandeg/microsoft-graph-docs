---
title: "Create deviceHealthScript"
description: "Create a new deviceHealthScript object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create deviceHealthScript

Namespace: microsoft.graph

Create a new [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceHealthScripts
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object.

The following table shows the properties that are required when you create the [deviceHealthScript](../resources/intune-devices-devicehealthscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|publisher|String|Name of the device health script publisher|
|version|String|Version of the device health script|
|displayName|String|Name of the device health script|
|description|String|Description of the device health script|
|detectionScriptContent|Binary|The entire content of the detection powershell script|
|remediationScriptContent|Binary|The entire content of the remediation powershell script|
|createdDateTime|DateTimeOffset|The timestamp of when the device health script was created. This property is read-only.|
|lastModifiedDateTime|DateTimeOffset|The timestamp of when the device health script was modified. This property is read-only.|
|runAsAccount|Enumeration|Indicates the type of execution context. Possible values are: `system`, `user`.|
|enforceSignatureCheck|Boolean|Indicate whether the script signature needs be checked|
|runAs32Bit|Boolean|Indicate whether PowerShell script(s) should run as 32-bit|
|roleScopeTagIds|String collection|List of Scope Tag IDs for the device health script|



## Response
If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/intune-devices-devicehealthscript.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicehealthscript_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/deviceHealthScripts
Content-type: application/json
Content-length: 485

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
  ]
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicehealthscript"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 656

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "aa148d30-8d30-aa14-308d-14aa308d14aa",
  "publisher": "Publisher value",
  "version": "Version value",
  "displayName": "Display Name value",
  "description": "Description value",
  "detectionScriptContent": "ZGV0ZWN0aW9uU2NyaXB0Q29udGVudA==",
  "remediationScriptContent": "cmVtZWRpYXRpb25TY3JpcHRDb250ZW50",
  "createdDateTime": "2017-01-01T00:02:37.446308+03:00",
  "lastModifiedDateTime": "2016-12-31T23:56:51.5562076+03:00",
  "runAsAccount": "String",
  "enforceSignatureCheck": true,
  "runAs32Bit": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```


---
title: "Create deviceHealthScripts"
description: "Create a new deviceHealthScripts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceHealthScripts

Namespace: microsoft.graph

Create a new deviceHealthScripts object.

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
POST /deviceManagement/deviceHealthScripts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceHealthScript](../resources/devicehealthscript.md) object.

The following table shows the properties that are required when you create the [deviceHealthScript](../resources/devicehealthscript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|publisher|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|detectionScriptContent|Binary|**TODO: Add Description**|
|remediationScriptContent|Binary|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|runAsAccount|runAsAccountType|**TODO: Add Description**. Possible values are: `system`, `user`.|
|enforceSignatureCheck|Boolean|**TODO: Add Description**|
|runAs32Bit|Boolean|**TODO: Add Description**|
|roleScopeTagIds|String collection|**TODO: Add Description**|
|isGlobalScript|Boolean|**TODO: Add Description**|
|highestAvailableVersion|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [deviceHealthScript](../resources/devicehealthscript.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicehealthscript_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts
Content-Type: application/json
Content-length: 458

{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "Binary",
  "remediationScriptContent": "Binary",
  "runAsAccount": "String",
  "enforceSignatureCheck": "Boolean",
  "runAs32Bit": "Boolean",
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": "Boolean",
  "highestAvailableVersion": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicehealthscript"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceHealthScript",
  "id": "408a589c-589c-408a-9c58-8a409c588a40",
  "publisher": "String",
  "version": "String",
  "displayName": "String",
  "description": "String",
  "detectionScriptContent": "Binary",
  "remediationScriptContent": "Binary",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "runAsAccount": "String",
  "enforceSignatureCheck": "Boolean",
  "runAs32Bit": "Boolean",
  "roleScopeTagIds": [
    "String"
  ],
  "isGlobalScript": "Boolean",
  "highestAvailableVersion": "String"
}
```


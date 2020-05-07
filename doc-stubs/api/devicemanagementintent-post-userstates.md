---
title: "Create userStates"
description: "Create a new userStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userStates

Namespace: microsoft.graph

Create a new userStates object.

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
POST /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object.

The following table shows the properties that are required when you create the [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|userPrincipalName|String|**TODO: Add Description**|
|userName|String|**TODO: Add Description**|
|deviceCount|Int32|**TODO: Add Description**|
|lastReportedDateTime|DateTimeOffset|**TODO: Add Description**|
|state|complianceStatus|**TODO: Add Description**. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|



## Response

If successful, this method returns a `201 Created` response code and a [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementintentuserstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
Content-Type: application/json
Content-length: 232

{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": "Integer",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementintentuserstate"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "dc4d03d9-03d9-dc4d-d903-4ddcd9034ddc",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": "Integer",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```


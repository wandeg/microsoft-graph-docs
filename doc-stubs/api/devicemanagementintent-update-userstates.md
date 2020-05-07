---
title: "Update userStates"
description: "Update the properties of a userStates object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userStates

Namespace: microsoft.graph

Update the properties of a userStates object.

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
PATCH /deviceManagement/intents/{deviceManagementIntentId}/userStates
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

If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntentUserState](../resources/devicemanagementintentuserstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userstates"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
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


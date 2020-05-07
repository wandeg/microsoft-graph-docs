---
title: "Add runSummary"
description: "Add runSummary by posting to the runSummary collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add runSummary

Namespace: microsoft.graph

Add runSummary by posting to the runSummary collection.

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
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object.

The following table shows the properties that are required when you create the [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the device management script run summary entity. This property is read-only.|
|successDeviceCount|Int32|Success device count.|
|errorDeviceCount|Int32|Error device count.|
|successUserCount|Int32|Success user count.|
|errorUserCount|Int32|Error user count.|



## Response

If successful, this method returns a `204 No Content` response code and a [deviceManagementScriptRunSummary](../resources/devicemanagementscriptrunsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementscriptrunsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/runSummary/$ref
Content-Type: application/json
Content-length: 228

{
  "@odata.type": "#microsoft.management.services.api.deviceManagementScriptRunSummary",
  "successDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "successUserCount": "Integer",
  "errorUserCount": "Integer"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.devicemanagementscriptrunsummary"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.management.services.api.deviceManagementScriptRunSummary",
  "id": "34f937b7-37b7-34f9-b737-f934b737f934",
  "successDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "successUserCount": "Integer",
  "errorUserCount": "Integer"
}
```


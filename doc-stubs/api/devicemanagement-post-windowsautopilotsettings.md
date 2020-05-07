---
title: "Create windowsAutopilotSettings"
description: "Create a new windowsAutopilotSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create windowsAutopilotSettings

Namespace: microsoft.graph

Create a new windowsAutopilotSettings object.

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
POST /deviceManagement/windowsAutopilotSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.

The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|**TODO: Add Description**|
|lastManualSyncTriggerDateTime|DateTimeOffset|**TODO: Add Description**|
|syncStatus|windowsAutopilotSyncStatus|**TODO: Add Description**. Possible values are: `unknown`, `inProgress`, `completed`, `failed`.|



## Response

If successful, this method returns a `201 Created` response code and a [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsautopilotsettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-Type: application/json
Content-length: 196

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsautopilotsettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "a4c56a85-6a85-a4c5-856a-c5a4856ac5a4",
  "lastSyncDateTime": "String (timestamp)",
  "lastManualSyncTriggerDateTime": "String (timestamp)",
  "syncStatus": "String"
}
```


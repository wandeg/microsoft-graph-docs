---
title: "Update windowsAutopilotSettings"
description: "Update the properties of a windowsAutopilotSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update windowsAutopilotSettings

Namespace: microsoft.graph

Update the properties of a [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.

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
PATCH /deviceManagement/windowsAutopilotSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.

The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Last data sync date time with DDS service.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Last data sync date time with DDS service.|
|syncStatus|windowsAutopilotSyncStatus|Indicates the status of sync with Device data sync (DDS) service. Possible values are: `unknown`, `inProgress`, `completed`, `failed`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windowsautopilotsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-Type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:58:06.732277+03:00",
  "syncStatus": "String"
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
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "df2f5067-5067-df2f-6750-2fdf67502fdf",
  "lastSyncDateTime": "2017-01-01T00:02:17.5414184+03:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:58:06.732277+03:00",
  "syncStatus": "String"
}
```


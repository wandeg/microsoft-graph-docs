---
title: "Create windowsAutopilotSettings"
description: "Create a new windowsAutopilotSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create windowsAutopilotSettings

Create a new [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.

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
POST ** Collection URI for microsoft.graph.windowsAutopilotSettings not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the windowsAutopilotSettings object.

The following table shows the properties that are required when you create the windowsAutopilotSettings.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Last data sync date time with DDS service.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Last data sync date time with DDS service.|
|syncStatus|Enumeration|Indicates the status of sync with Device data sync (DDS) service. Possible values are: `unknown`, `inProgress`, `completed`, `failed`.|



## Response
If successful, this method returns a `201 Created` response code and a [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_windowsautopilotsettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.windowsAutopilotSettings not found
Content-type: application/json
Content-length: 225

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2016-12-31T23:59:56.035751+03:00",
  "lastManualSyncTriggerDateTime": "2017-01-01T00:03:25.7339534+03:00",
  "syncStatus": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsautopilotsettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 274

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "06cf0f21-0f21-06cf-210f-cf06210fcf06",
  "lastSyncDateTime": "2016-12-31T23:59:56.035751+03:00",
  "lastManualSyncTriggerDateTime": "2017-01-01T00:03:25.7339534+03:00",
  "syncStatus": "String"
}
```


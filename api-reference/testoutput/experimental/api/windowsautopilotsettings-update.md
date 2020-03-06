---
title: "Update windowsAutopilotSettings"
description: "Update the properties of a windowsAutopilotSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update windowsAutopilotSettings

Namespace: microsoft.graph

Update the properties of a [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.

The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastSyncDateTime|DateTimeOffset|Last data sync date time with DDS service.|
|lastManualSyncTriggerDateTime|DateTimeOffset|Last data sync date time with DDS service.|
|syncStatus|Enumeration|Indicates the status of sync with Device data sync (DDS) service. Possible values are: `unknown`, `inProgress`, `completed`, `failed`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_windowsautopilotsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 226

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2016-12-31T23:56:56.1979703+03:00",
  "lastManualSyncTriggerDateTime": "2017-01-01T00:01:23.5386669+03:00",
  "syncStatus": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "ae112b40-2b40-ae11-402b-11ae402b11ae",
  "lastSyncDateTime": "2016-12-31T23:56:56.1979703+03:00",
  "lastManualSyncTriggerDateTime": "2017-01-01T00:01:23.5386669+03:00",
  "syncStatus": "String"
}
```


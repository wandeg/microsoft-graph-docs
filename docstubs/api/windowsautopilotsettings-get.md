---
title: "Get windowsAutopilotSettings"
description: "Read properties and relationships of the windowsAutopilotSettings object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsAutopilotSettings

Namespace: microsoft.graph

Read properties and relationships of the [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object.

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
GET /deviceManagement/windowsAutopilotSettings
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [windowsAutopilotSettings](../resources/windowsautopilotsettings.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsautopilotsettings"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsAutopilotSettings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 304

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
    "id": "2f6f3905-3905-2f6f-0539-6f2f05396f2f",
    "lastSyncDateTime": "2017-01-01T00:01:32.4757974+03:00",
    "lastManualSyncTriggerDateTime": "2017-01-01T00:02:39.2916739+03:00",
    "syncStatus": "String"
  }
}
```


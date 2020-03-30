---
title: "Get windowsInformationProtectionWipeAction"
description: "Read properties and relationships of the windowsInformationProtectionWipeAction object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get windowsInformationProtectionWipeAction

Namespace: microsoft.graph

Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.

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
GET /deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
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
If successful, this method returns a `200 OK` response code and [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_windowsinformationprotectionwipeaction"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsInformationProtectionWipeActions/{windowsInformationProtectionWipeActionId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
    "id": "e062947c-947c-e062-7c94-62e07c9462e0",
    "status": "String",
    "targetedUserId": "Targeted User Id value",
    "targetedDeviceRegistrationId": "Targeted Device Registration Id value",
    "targetedDeviceName": "Targeted Device Name value",
    "targetedDeviceMacAddress": "Targeted Device Mac Address value",
    "lastCheckInDateTime": "2017-01-01T00:03:24.7233796+03:00"
  }
}
```


---
title: "Update deviceManagementTroubleshootingEvents"
description: "Update the properties of a deviceManagementTroubleshootingEvents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceManagementTroubleshootingEvents

Namespace: microsoft.graph

Update the properties of a deviceManagementTroubleshootingEvents object.

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
PATCH /me/deviceManagementTroubleshootingEvents
PATCH /users/{usersId}/deviceManagementTroubleshootingEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|correlationId|String|Id used for tracing the failure in the service.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementtroubleshootingevents"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/deviceManagementTroubleshootingEvents
Content-Type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2016-12-31T23:57:29.3002453+03:00",
  "correlationId": "Correlation Id value"
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
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "2d938bbf-8bbf-2d93-bf8b-932dbf8b932d",
  "eventDateTime": "2016-12-31T23:57:29.3002453+03:00",
  "correlationId": "Correlation Id value"
}
```


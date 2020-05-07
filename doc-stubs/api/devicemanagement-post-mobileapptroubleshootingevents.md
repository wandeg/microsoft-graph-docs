---
title: "Create mobileAppTroubleshootingEvents"
description: "Create a new mobileAppTroubleshootingEvents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create mobileAppTroubleshootingEvents

Namespace: microsoft.graph

Create a new mobileAppTroubleshootingEvents object.

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
POST /deviceManagement/mobileAppTroubleshootingEvents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object.

The following table shows the properties that are required when you create the [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The GUID for the object|



## Response

If successful, this method returns a `201 Created` response code and a [mobileAppTroubleshootingEvent](../resources/mobileapptroubleshootingevent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_mobileapptroubleshootingevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents
Content-Type: application/json
Content-length: 89

{
  "@odata.type": "#microsoft.management.services.api.mobileAppTroubleshootingEvent"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.mobileapptroubleshootingevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.management.services.api.mobileAppTroubleshootingEvent",
  "id": "791d4da0-4da0-791d-a04d-1d79a04d1d79"
}
```


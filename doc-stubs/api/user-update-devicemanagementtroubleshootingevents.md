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
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|eventDateTime|DateTimeOffset|**TODO: Add Description**|
|correlationId|String|**TODO: Add Description**|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/devicemanagementtroubleshootingerrordetails.md)|**TODO: Add Description**|
|eventName|String|**TODO: Add Description**|
|additionalInformation|[keyValuePair](../resources/keyvaluepair.md) collection|**TODO: Add Description**|



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
Content-length: 403

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
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
  "id": "80814466-4466-8081-6644-818066448180",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
  },
  "eventName": "String",
  "additionalInformation": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ]
}
```


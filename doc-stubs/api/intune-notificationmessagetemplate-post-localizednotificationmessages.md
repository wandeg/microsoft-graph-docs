---
title: "Create localizedNotificationMessages"
description: "Create a new localizedNotificationMessages object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create localizedNotificationMessages

Namespace: microsoft.graph

Create a new localizedNotificationMessages object.

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
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [localizedNotificationMessage](../resources/intune-localizednotificationmessage.md) object.

The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-localizednotificationmessage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|locale|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|messageTemplate|String|**TODO: Add Description**|
|isDefault|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-localizednotificationmessage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_localizednotificationmessage_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-Type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": "Boolean"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.localizednotificationmessage"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "c41598b0-98b0-c415-b098-15c4b09815c4",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": "Boolean"
}
```


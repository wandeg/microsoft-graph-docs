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
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [localizedNotificationMessage](../resources/localizednotificationmessage.md) object.

The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/localizednotificationmessage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|locale|String|The Locale for which this message is destined.|
|subject|String|The Message Template Subject.|
|messageTemplate|String|The Message Template content.|
|isDefault|Boolean|Flag to indicate whether or not this is the default locale for language fallback. This flag can only be set. To unset, set this property to true on another Localized Notification Message.|



## Response
If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/localizednotificationmessage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_localizednotificationmessage_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-Type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
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
  "id": "cf36839e-839e-cf36-9e83-36cf9e8336cf",
  "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```


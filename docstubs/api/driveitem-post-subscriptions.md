---
title: "Add subscriptions"
description: "Add subscriptions by posting to the subscriptions collection."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add subscriptions

Namespace: microsoft.graph

Add subscriptions by posting to the subscriptions collection.

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
POST /workbooks/{workbooksId}/subscriptions/$ref
POST /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/subscriptions/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [subscription](../resources/subscription.md) object.

The following table shows the properties that are required when you create the [subscription](../resources/subscription.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|resource|String|**TODO: Add Description**|
|changeType|String|**TODO: Add Description**|
|clientState|String|**TODO: Add Description**|
|notificationUrl|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|applicationId|String|**TODO: Add Description**|
|creatorId|String|**TODO: Add Description**|
|includeProperties|Boolean|**TODO: Add Description**|
|includeResourceData|Boolean|**TODO: Add Description**|
|lifecycleNotificationUrl|String|**TODO: Add Description**|
|encryptionCertificate|String|**TODO: Add Description**|
|encryptionCertificateId|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/subscriptions
Content-Type: application/json
Content-length: 636

{
  "@odata.type": "#microsoft.graph.subscription",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2016-12-31T23:57:13.9832195+03:00",
  "applicationId": "Application Id value",
  "creatorId": "Creator Id value",
  "includeProperties": true,
  "includeResourceData": true,
  "lifecycleNotificationUrl": "https://example.com/lifecycleNotificationUrl/",
  "encryptionCertificate": "Encryption Certificate value",
  "encryptionCertificateId": "Encryption Certificate Id value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "858248a6-48a6-8582-a648-8285a6488285",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2016-12-31T23:57:13.9832195+03:00",
  "applicationId": "Application Id value",
  "creatorId": "Creator Id value",
  "includeProperties": true,
  "includeResourceData": true,
  "lifecycleNotificationUrl": "https://example.com/lifecycleNotificationUrl/",
  "encryptionCertificate": "Encryption Certificate value",
  "encryptionCertificateId": "Encryption Certificate Id value"
}
```


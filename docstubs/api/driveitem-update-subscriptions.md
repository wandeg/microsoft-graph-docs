---
title: "Update subscriptions"
description: "Update the properties of a subscriptions object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update subscriptions

Namespace: microsoft.graph

Update the properties of a subscriptions object.

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
PATCH /workbooks/{workbooksId}/subscriptions
PATCH /invitations/{invitationsId}/invitedUser/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/subscriptions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
If successful, this method returns a `200 OK` response code and an updated [subscription](../resources/subscription.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_subscriptions"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/workbooks/{workbooksId}/subscriptions
Content-Type: application/json
Content-length: 636

{
  "@odata.type": "#microsoft.graph.subscription",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
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
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "279fbc78-bc78-279f-78bc-9f2778bc9f27",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2016-12-31T23:59:10.7331181+03:00",
  "applicationId": "Application Id value",
  "creatorId": "Creator Id value",
  "includeProperties": true,
  "includeResourceData": true,
  "lifecycleNotificationUrl": "https://example.com/lifecycleNotificationUrl/",
  "encryptionCertificate": "Encryption Certificate value",
  "encryptionCertificateId": "Encryption Certificate Id value"
}
```


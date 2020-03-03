---
title: "Update subscription"
description: "Update the properties of a subscription object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update subscription

Update the properties of a [subscription](../resources/subscription.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /subscriptions/{subscriptionsId}
PATCH /workbooks/{workbooksId}/subscriptions/{subscriptionId}
PATCH /me/joinedGroups/{groupId}/drive/list/subscriptions/{subscriptionId}
PATCH /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/subscriptions/{subscriptionId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [subscription](../resources/subscription.md) object.

The following table shows the properties that are required when you create the [subscription](../resources/subscription.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|resource|String||
|changeType|String||
|clientState|String||
|notificationUrl|String||
|expirationDateTime|DateTimeOffset||
|applicationId|String||
|creatorId|String||
|includeProperties|Boolean||
|includeResourceData|Boolean||
|lifecycleNotificationUrl|String||
|encryptionCertificate|String||
|encryptionCertificateId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [subscription](../resources/subscription.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_subscription"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/subscriptions/{subscriptionsId}
Content-type: application/json
Content-length: 635

{
  "@odata.type": "#microsoft.graph.subscription",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2017-01-01T00:01:09.280378+03:00",
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 684

{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "aedfa54d-a54d-aedf-4da5-dfae4da5dfae",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2017-01-01T00:01:09.280378+03:00",
  "applicationId": "Application Id value",
  "creatorId": "Creator Id value",
  "includeProperties": true,
  "includeResourceData": true,
  "lifecycleNotificationUrl": "https://example.com/lifecycleNotificationUrl/",
  "encryptionCertificate": "Encryption Certificate value",
  "encryptionCertificateId": "Encryption Certificate Id value"
}
```


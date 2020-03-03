---
title: "Add subscriptions"
description: "Add subscriptions by posting to the subscriptions collection."
author: ""
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
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/joinedGroups/{groupId}/drive/list/subscriptions/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/joinedGroups/{groupId}/drive/list/subscriptions
Content-type: application/json
Content-length: 636

{
  "@odata.type": "#microsoft.graph.subscription",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
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
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 685

{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "ccd590a4-90a4-ccd5-a490-d5cca490d5cc",
  "resource": "Resource value",
  "changeType": "Change Type value",
  "clientState": "Client State value",
  "notificationUrl": "https://example.com/notificationUrl/",
  "expirationDateTime": "2016-12-31T23:59:56.1430588+03:00",
  "applicationId": "Application Id value",
  "creatorId": "Creator Id value",
  "includeProperties": true,
  "includeResourceData": true,
  "lifecycleNotificationUrl": "https://example.com/lifecycleNotificationUrl/",
  "encryptionCertificate": "Encryption Certificate value",
  "encryptionCertificateId": "Encryption Certificate Id value"
}
```


---
title: "List subscriptions"
description: "List properties and relationships of the subscription objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List subscriptions

Namespace: microsoft.graph

List properties and relationships of the [subscription](../resources/subscription.md) objects.

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
GET /subscriptions
GET /workbooks/{workbooksId}/subscriptions
GET /me/joinedGroups/{groupId}/drive/list/subscriptions
GET /me/joinedGroups/{groupId}/drive/activities/{itemActivityOLDId}/driveItem/subscriptions
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
If successful, this method returns a `200 OK` response code and a collection of [subscription](../resources/subscription.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_subscription"
}
-->
``` http
GET https://graph.microsoft.com/beta/subscriptions
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.subscription)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 848

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.subscription",
      "id": "8375e5ab-e5ab-8375-abe5-7583abe57583",
      "resource": "Resource value",
      "changeType": "Change Type value",
      "clientState": "Client State value",
      "notificationUrl": "https://example.com/notificationUrl/",
      "expirationDateTime": "2016-12-31T23:56:24.5775752+00:00",
      "applicationId": "Application Id value",
      "creatorId": "Creator Id value",
      "includeProperties": true,
      "includeResourceData": true,
      "lifecycleNotificationUrl": "https://example.com/lifecycleNotificationUrl/",
      "encryptionCertificate": "Encryption Certificate value",
      "encryptionCertificateId": "Encryption Certificate Id value",
      "latestSupportedTlsVersion": "Latest Supported Tls Version value"
    }
  ]
}
```


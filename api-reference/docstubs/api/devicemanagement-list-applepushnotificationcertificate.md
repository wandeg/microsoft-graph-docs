---
title: "List applePushNotificationCertificate"
description: "Get the applePushNotificationCertificates from the applePushNotificationCertificate navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List applePushNotificationCertificate

Namespace: microsoft.graph

Get the applePushNotificationCertificates from the applePushNotificationCertificate navigation property.

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
GET /deviceManagement/applePushNotificationCertificate
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [applePushNotificationCertificate](../resources/applepushnotificationcertificate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_applepushnotificationcertificate"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/applePushNotificationCertificate
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.applepushnotificationcertificate)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.applePushNotificationCertificate",
      "id": "cbbf7336-7336-cbbf-3673-bfcb3673bfcb",
      "appleIdentifier": "Apple Identifier value",
      "topicIdentifier": "Topic Identifier value",
      "lastModifiedDateTime": "2016-12-31T23:58:12.0125666+00:00",
      "expirationDateTime": "2017-01-01T00:00:55.8131541+00:00",
      "certificate": "Certificate value"
    }
  ]
}
```


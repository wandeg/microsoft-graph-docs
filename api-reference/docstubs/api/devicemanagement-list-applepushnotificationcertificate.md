---
title: "List applePushNotificationCertificate"
description: "Get the applePushNotificationCertificates from the applePushNotificationCertificate navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
**Note:** The response object shown here might be shortened for readability.
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
      "id": "b63e766d-766d-b63e-6d76-3eb66d763eb6",
      "appleIdentifier": "Apple Identifier value",
      "topicIdentifier": "Topic Identifier value",
      "lastModifiedDateTime": "2017-01-01T00:02:46.687785+03:00",
      "expirationDateTime": "2016-12-31T23:58:13.22093+03:00",
      "certificate": "Certificate value"
    }
  ]
}
```


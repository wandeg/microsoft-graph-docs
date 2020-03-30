---
title: "Update dataSharingConsent"
description: "Update the properties of a dataSharingConsent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update dataSharingConsent

Namespace: microsoft.graph

Update the properties of a [dataSharingConsent](../resources/datasharingconsent.md) object.

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
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [dataSharingConsent](../resources/datasharingconsent.md) object.

The following table shows the properties that are required when you create the [dataSharingConsent](../resources/datasharingconsent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|serviceDisplayName|String||
|termsUrl|String||
|granted|Boolean||
|grantDateTime|DateTimeOffset||
|grantedByUpn|String||
|grantedByUserId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/datasharingconsent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_datasharingconsent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-type: application/json
Content-length: 333

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:57:21.8695044+03:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
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
Content-Length: 382

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "7d150692-0692-7d15-9206-157d9206157d",
  "serviceDisplayName": "Service Display Name value",
  "termsUrl": "https://example.com/termsUrl/",
  "granted": true,
  "grantDateTime": "2016-12-31T23:57:21.8695044+03:00",
  "grantedByUpn": "Granted By Upn value",
  "grantedByUserId": "Granted By User Id value"
}
```


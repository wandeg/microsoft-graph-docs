---
title: "List dataSharingConsents"
description: "Get the dataSharingConsents from the dataSharingConsents navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List dataSharingConsents

Namespace: microsoft.graph

Get the dataSharingConsents from the dataSharingConsents navigation property.

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
GET /deviceManagement/dataSharingConsents
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
If successful, this method returns a `200 OK` response code and a collection of [dataSharingConsent](../resources/datasharingconsent.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_datasharingconsent"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.datasharingconsent)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 447

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.dataSharingConsent",
      "id": "aa4ff184-f184-aa4f-84f1-4faa84f14faa",
      "serviceDisplayName": "Service Display Name value",
      "termsUrl": "https://example.com/termsUrl/",
      "granted": true,
      "grantDateTime": "2016-12-31T23:56:27.1882715+03:00",
      "grantedByUpn": "Granted By Upn value",
      "grantedByUserId": "Granted By User Id value"
    }
  ]
}
```


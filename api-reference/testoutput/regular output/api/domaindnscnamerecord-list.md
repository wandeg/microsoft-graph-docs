---
title: "List domainDnsCnameRecords"
description: "List properties and relationships of the domainDnsCnameRecord objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List domainDnsCnameRecords

Namespace: microsoft.graph

List properties and relationships of the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) objects.

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
GET ** Collection URI for microsoft.graph.domainDnsCnameRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnscnamerecord"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.domainDnsCnameRecord not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domaindnscnamerecord)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 371

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domainDnsCnameRecord",
      "id": "7741e4a4-e4a4-7741-a4e4-4177a4e44177",
      "isOptional": true,
      "label": "Label value",
      "recordType": "Record Type value",
      "supportedService": "Supported Service value",
      "ttl": 3,
      "canonicalName": "Canonical Name value"
    }
  ]
}
```


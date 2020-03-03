---
title: "List domainDnsRecords"
description: "List properties and relationships of the domainDnsRecord objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List domainDnsRecords

Namespace: microsoft.graph

List properties and relationships of the [domainDnsRecord](../resources/domaindnsrecord.md) objects.

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
GET /domainDnsRecords
GET /domains/{domainsId}/verificationDnsRecords
GET /domains/{domainsId}/serviceConfigurationRecords
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnsrecord"
}
-->
``` http
GET https://graph.microsoft.com/localtest/domainDnsRecords
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domaindnsrecord)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 318

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domainDnsRecord",
      "id": "9bc3fc52-fc52-9bc3-52fc-c39b52fcc39b",
      "isOptional": true,
      "label": "Label value",
      "recordType": "Record Type value",
      "supportedService": "Supported Service value",
      "ttl": 3
    }
  ]
}
```


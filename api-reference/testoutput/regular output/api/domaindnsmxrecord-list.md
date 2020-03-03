---
title: "List domainDnsMxRecords"
description: "List properties and relationships of the domainDnsMxRecord objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List domainDnsMxRecords

List properties and relationships of the [domainDnsMxRecord](../resources/domaindnsmxrecord.md) objects.

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
GET ** Collection URI for microsoft.graph.domainDnsMxRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [domainDnsMxRecord](../resources/domaindnsmxrecord.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnsmxrecord"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.domainDnsMxRecord not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.domaindnsmxrecord)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.domainDnsMxRecord",
      "id": "c2ae9acc-9acc-c2ae-cc9a-aec2cc9aaec2",
      "isOptional": true,
      "label": "Label value",
      "recordType": "Record Type value",
      "supportedService": "Supported Service value",
      "ttl": 3,
      "mailExchange": "Mail Exchange value",
      "preference": 10
    }
  ]
}
```


---
title: "Get domainDnsSrvRecord"
description: "Read properties and relationships of the domainDnsSrvRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get domainDnsSrvRecord

Namespace: microsoft.graph

Read properties and relationships of the [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.

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
GET ** Entity URI for microsoft.graph.domainDnsSrvRecord not found
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnssrvrecord"
}
-->
``` http
GET https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.domainDnsSrvRecord not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 455

{
  "value": {
    "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
    "id": "7a27ed2b-ed2b-7a27-2bed-277a2bed277a",
    "isOptional": true,
    "label": "Label value",
    "recordType": "Record Type value",
    "supportedService": "Supported Service value",
    "ttl": 3,
    "nameTarget": "Name Target value",
    "port": 4,
    "priority": 8,
    "protocol": "Protocol value",
    "service": "Service value",
    "weight": 6
  }
}
```


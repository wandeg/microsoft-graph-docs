---
title: "Get domainDnsCnameRecord"
description: "Read properties and relationships of the domainDnsCnameRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get domainDnsCnameRecord

Read properties and relationships of the [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object.

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
GET ** Entity URI for microsoft.graph.domainDnsCnameRecord not found
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
If successful, this method returns a `200 OK` response code and [domainDnsCnameRecord](../resources/domaindnscnamerecord.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_domaindnscnamerecord"
}
-->
``` http
GET https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.domainDnsCnameRecord not found
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 341

{
  "value": {
    "@odata.type": "#microsoft.graph.domainDnsCnameRecord",
    "id": "e5698887-8887-e569-8788-69e5878869e5",
    "isOptional": true,
    "label": "Label value",
    "recordType": "Record Type value",
    "supportedService": "Supported Service value",
    "ttl": 3,
    "canonicalName": "Canonical Name value"
  }
}
```


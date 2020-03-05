---
title: "Update domainDnsTxtRecord"
description: "Update the properties of a domainDnsTxtRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update domainDnsTxtRecord

Namespace: microsoft.graph

Update the properties of a [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.

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
PATCH ** Entity URI for microsoft.graph.domainDnsTxtRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.

The following table shows the properties that are required when you create the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|text|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_domaindnstxtrecord"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.domainDnsTxtRecord not found
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.domainDnsTxtRecord",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3,
  "text": "Text value"
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
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.domainDnsTxtRecord",
  "id": "4bf7a598-a598-4bf7-98a5-f74b98a5f74b",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3,
  "text": "Text value"
}
```


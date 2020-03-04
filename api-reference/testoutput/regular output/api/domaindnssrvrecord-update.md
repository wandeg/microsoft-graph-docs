---
title: "Update domainDnsSrvRecord"
description: "Update the properties of a domainDnsSrvRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update domainDnsSrvRecord

Namespace: microsoft.graph

Update the properties of a [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.

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
PATCH ** Entity URI for microsoft.graph.domainDnsSrvRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.

The following table shows the properties that are required when you create the [domainDnsSrvRecord](../resources/domaindnssrvrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|nameTarget|String||
|port|Int32||
|priority|Int32||
|protocol|String||
|service|String||
|weight|Int32||



## Response
If successful, this method returns a `200 OK` response code and an updated [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_domaindnssrvrecord"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest** Entity URI for microsoft.graph.domainDnsSrvRecord not found
Content-type: application/json
Content-length: 361

{
  "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
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
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
  "id": "c1f54f89-4f89-c1f5-894f-f5c1894ff5c1",
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
```


---
title: "Create domainDnsSrvRecord"
description: "Create a new domainDnsSrvRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create domainDnsSrvRecord

Namespace: microsoft.graph

Create a new [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.

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
POST ** Collection URI for microsoft.graph.domainDnsSrvRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_domaindnssrvrecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.domainDnsSrvRecord not found
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
  "truncated": true,
  "@odata.type": "microsoft.graph.domaindnssrvrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 410

{
  "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
  "id": "40b5d338-d338-40b5-38d3-b54038d3b540",
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


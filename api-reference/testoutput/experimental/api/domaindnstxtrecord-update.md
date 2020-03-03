---
title: "Update domainDnsTxtRecord"
description: "Update the properties of a domainDnsTxtRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update domainDnsTxtRecord

Update the properties of a [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object.

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
PATCH ** Entity URI for microsoft.graph.domainDnsTxtRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [domainDnsTxtRecord](../resources/domainDnsTxtRecord.md) object.

The following table shows the properties that are required when you create the [domainDnsTxtRecord](../resources/domaindnstxtrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|text|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [domainDnsTxtRecord](../resources/domaindnstxtrecord.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_domaindnstxtrecord"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api** Entity URI for microsoft.graph.domainDnsTxtRecord not found
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
  "id": "25c45303-5303-25c4-0353-c4250353c425",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3,
  "text": "Text value"
}
```


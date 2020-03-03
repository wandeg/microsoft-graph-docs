---
title: "Create domainDnsUnavailableRecord"
description: "Create a new domainDnsUnavailableRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create domainDnsUnavailableRecord

Create a new [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.

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
POST ** Collection URI for microsoft.graph.domainDnsUnavailableRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the domainDnsUnavailableRecord object.

The following table shows the properties that are required when you create the domainDnsUnavailableRecord.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domainDnsRecord.md)|
|description|String||



## Response
If successful, this method returns a `201 Created` response code and a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_domaindnsunavailablerecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/docs\api** Collection URI for microsoft.graph.domainDnsUnavailableRecord not found
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.domainDnsUnavailableRecord",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3,
  "description": "Description value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domaindnsunavailablerecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.domainDnsUnavailableRecord",
  "id": "9cc75253-5253-9cc7-5352-c79c5352c79c",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3,
  "description": "Description value"
}
```


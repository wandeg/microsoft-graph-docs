---
title: "Create domainDnsMxRecord"
description: "Create a new domainDnsMxRecord object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create domainDnsMxRecord

Namespace: microsoft.graph

Create a new [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.

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
POST ** Collection URI for microsoft.graph.domainDnsMxRecord not found
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object.

The following table shows the properties that are required when you create the [domainDnsMxRecord](../resources/domaindnsmxrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|recordType|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32| Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|mailExchange|String||
|preference|Int32||



## Response
If successful, this method returns a `201 Created` response code and a [domainDnsMxRecord](../resources/domaindnsmxrecord.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_domaindnsmxrecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest** Collection URI for microsoft.graph.domainDnsMxRecord not found
Content-type: application/json
Content-length: 273

{
  "@odata.type": "#microsoft.graph.domainDnsMxRecord",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3,
  "mailExchange": "Mail Exchange value",
  "preference": 10
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domaindnsmxrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 322

{
  "@odata.type": "#microsoft.graph.domainDnsMxRecord",
  "id": "bd7e6eba-6eba-bd7e-ba6e-7ebdba6e7ebd",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3,
  "mailExchange": "Mail Exchange value",
  "preference": 10
}
```


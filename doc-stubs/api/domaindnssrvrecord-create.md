---
title: "Create domainDnsSrvRecord"
description: "Create a new domainDnsSrvRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create domainDnsSrvRecord
Namespace: microsoft.graph

Create a new [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.domainDnsSrvRecord not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object.

The following table shows the properties that are required when you create the [domainDnsSrvRecord](../resources/domaindnssrvrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|label|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|recordType|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|supportedService|String|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|ttl|Int32|**TODO: Add Description** Inherited from [domainDnsRecord](../resources/domaindnsrecord.md)|
|nameTarget|String|**TODO: Add Description**|
|port|Int32|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|protocol|String|**TODO: Add Description**|
|service|String|**TODO: Add Description**|
|weight|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [domainDnsSrvRecord](../resources/domaindnssrvrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_domaindnssrvrecord_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.domainDnsSrvRecord not found
Content-Type: application/json
Content-length: 339

{
  "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "nameTarget": "String",
  "port": "Integer",
  "priority": "Integer",
  "protocol": "String",
  "service": "String",
  "weight": "Integer"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domaindnssrvrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.domainDnsSrvRecord",
  "id": "22b4529c-529c-22b4-9c52-b4229c52b422",
  "isOptional": "Boolean",
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": "Integer",
  "nameTarget": "String",
  "port": "Integer",
  "priority": "Integer",
  "protocol": "String",
  "service": "String",
  "weight": "Integer"
}
```


---
title: "Create verificationDnsRecords"
description: "Create a new verificationDnsRecords object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create verificationDnsRecords

Namespace: microsoft.graph

Create a new verificationDnsRecords object.

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
POST /domains/{domainsId}/verificationDnsRecords
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [domainDnsRecord](../resources/domaindnsrecord.md) object.

The following table shows the properties that are required when you create the [domainDnsRecord](../resources/domaindnsrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isOptional|Boolean|**TODO: Add Description**|
|label|String|**TODO: Add Description**|
|recordType|String|**TODO: Add Description**|
|supportedService|String|**TODO: Add Description**|
|ttl|Int32|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [domainDnsRecord](../resources/domaindnsrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_domaindnsrecord_from_domaindnsrecords"
}
-->
``` http
POST https://graph.microsoft.com/beta/domains/{domainsId}/verificationDnsRecords
Content-Type: application/json
Content-length: 208

{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domaindnsrecord"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "id": "0da20e32-0e32-0da2-320e-a20d320ea20d",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3
}
```


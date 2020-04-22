---
title: "Update verificationDnsRecords"
description: "Update the properties of a verificationDnsRecords object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update verificationDnsRecords

Namespace: microsoft.graph

Update the properties of a verificationDnsRecords object.

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
PATCH /domains/{domainsId}/verificationDnsRecords
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [domainDnsRecord](../resources/domaindnsrecord.md) object.

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
If successful, this method returns a `200 OK` response code and an updated [domainDnsRecord](../resources/domaindnsrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_verificationdnsrecords"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/domains/{domainsId}/verificationDnsRecords
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
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.domainDnsRecord",
  "id": "0ee1e06b-e06b-0ee1-6be0-e10e6be0e10e",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3
}
```


---
title: "Update domainDnsRecord"
description: "Update the properties of a domainDnsRecord object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update domainDnsRecord

Namespace: Microsoft.DirectoryServices

Update the properties of a [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object.

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
PATCH /domainDnsRecords/{domainDnsRecordsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object.

The following table shows the properties that are required when you create the [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|isOptional|Boolean|**TODO: Add Description**|
|label|String|**TODO: Add Description**|
|recordType|String|**TODO: Add Description**|
|supportedService|String|**TODO: Add Description**|
|ttl|Int32|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [domainDnsRecord](../resources/microsoft.directoryservices-domaindnsrecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_domaindnsrecord"
}
-->
``` http
PATCH https://graph.microsoft.com/changelog/domainDnsRecords/{domainDnsRecordsId}
Content-Type: application/json
Content-length: 220

{
  "@odata.type": "#Microsoft.DirectoryServices.domainDnsRecord",
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
  "@odata.type": "#Microsoft.DirectoryServices.domainDnsRecord",
  "id": "27d0adec-adec-27d0-ecad-d027ecadd027",
  "isOptional": true,
  "label": "Label value",
  "recordType": "Record Type value",
  "supportedService": "Supported Service value",
  "ttl": 3
}
```


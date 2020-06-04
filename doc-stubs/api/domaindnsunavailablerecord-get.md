---
title: "Get domainDnsUnavailableRecord"
description: "Read the properties and relationships of a domainDnsUnavailableRecord object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get domainDnsUnavailableRecord
Namespace: microsoft.graph

Read the properties and relationships of a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object.

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
GET /domainDnsUnavailableRecord
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [domainDnsUnavailableRecord](../resources/domaindnsunavailablerecord.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_domaindnsunavailablerecord"
}
-->
``` http
GET https://graph.microsoft.com/beta/domainDnsUnavailableRecord
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.domainDnsUnavailableRecord",
    "id": "b8530a83-0a83-b853-830a-53b8830a53b8",
    "isOptional": "Boolean",
    "label": "String",
    "recordType": "String",
    "supportedService": "String",
    "ttl": "Integer",
    "description": "String"
  }
}
```


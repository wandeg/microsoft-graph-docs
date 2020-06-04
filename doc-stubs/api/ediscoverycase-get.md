---
title: "Get ediscoveryCase"
description: "Read the properties and relationships of an ediscoveryCase object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get ediscoveryCase
Namespace: microsoft.graph

Read the properties and relationships of an [ediscoveryCase](../resources/ediscoverycase.md) object.

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
GET /cases/{casesId}
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

If successful, this method returns a `200 OK` response code and an [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_ediscoverycase"
}
-->
``` http
GET https://graph.microsoft.com/beta/cases/{casesId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoveryCase"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.ediscoveryCase",
    "id": "359e5635-5635-359e-3556-9e3535569e35",
    "description": "String",
    "createdBy": "String",
    "lastModifiedBy": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "status": "String",
    "closedBy": "String",
    "closedDateTime": "String (timestamp)",
    "externalId": "String",
    "displayName": "String",
    "createdDateTime": "String (timestamp)"
  }
}
```


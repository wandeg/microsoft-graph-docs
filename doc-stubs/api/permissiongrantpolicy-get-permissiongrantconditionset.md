---
title: "Get excludes"
description: "Read the properties and relationships of a permissionGrantConditionSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get excludes
Namespace: microsoft.graph

Read the properties and relationships of a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object.

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
GET /permissionGrantPolicy/excludes
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

If successful, this method returns a `200 OK` response code and a [permissionGrantConditionSet](../resources/permissiongrantconditionset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_permissiongrantconditionset"
}
-->
``` http
GET https://graph.microsoft.com/beta/permissionGrantPolicy/excludes
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permissionGrantConditionSet"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.permissionGrantConditionSet",
    "id": "c1c9cd6d-cd6d-c1c9-6dcd-c9c16dcdc9c1",
    "permissionClassification": "String",
    "permissionType": "String",
    "resourceApplication": "String",
    "permissions": [
      "String"
    ],
    "clientApplicationIds": [
      "String"
    ],
    "clientApplicationTenantIds": [
      "String"
    ],
    "clientApplicationPublisherIds": [
      "String"
    ],
    "clientApplicationsFromVerifiedPublisherOnly": "Boolean"
  }
}
```


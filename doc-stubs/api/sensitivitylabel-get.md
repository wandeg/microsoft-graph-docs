---
title: "Get sensitivityLabel"
description: "Read the properties and relationships of a sensitivityLabel object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get sensitivityLabel

Namespace: microsoft.graph

Read the properties and relationships of a [sensitivityLabel](../resources/sensitivitylabel.md) object.

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
GET /dataClassification/sensitivityLabels/{sensitivityLabelId}
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

If successful, this method returns a `200 OK` response code and a [sensitivityLabel](../resources/sensitivitylabel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sensitivitylabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/sensitivityLabels/{sensitivityLabelId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sensitivityLabel"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.sensitivityLabel",
    "id": "ef55db95-db95-ef55-95db-55ef95db55ef",
    "name": "String",
    "displayName": "String",
    "description": "String",
    "toolTip": "String",
    "isEndpointProtectionEnabled": "Boolean",
    "isDefault": "Boolean",
    "applicationMode": "String",
    "labelActions": [
      {
        "@odata.type": "microsoft.graph.encryptWithUserDefinedRights"
      }
    ],
    "assignedPolicies": [
      {
        "@odata.type": "microsoft.graph.labelPolicy"
      }
    ],
    "priority": "Integer",
    "autoLabeling": {
      "@odata.type": "microsoft.graph.autoLabeling"
    },
    "applicableTo": "String"
  }
}
```


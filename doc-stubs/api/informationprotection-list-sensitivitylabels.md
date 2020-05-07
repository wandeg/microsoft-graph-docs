---
title: "List sensitivityLabels"
description: "Get the sensitivityLabels from the sensitivityLabels navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List sensitivityLabels

Namespace: microsoft.graph

Get the sensitivityLabels from the sensitivityLabels navigation property.

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
GET /users/{usersId}/informationProtection/sensitivityLabels
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

If successful, this method returns a `200 OK` response code and a collection of [sensitivityLabel](../resources/sensitivitylabel.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_sensitivitylabel"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/informationProtection/sensitivityLabels
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.sensitivitylabel)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
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
  ]
}
```


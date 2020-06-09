---
title: "Get conditionalAccessPolicy"
description: "Read the properties and relationships of a conditionalAccessPolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get conditionalAccessPolicy
Namespace: microsoft.graph

Read the properties and relationships of a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object.

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
GET /policies/conditionalAccessPolicies/{conditionalAccessPolicyId}
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

If successful, this method returns a `200 OK` response code and a [conditionalAccessPolicy](../resources/conditionalaccesspolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicy"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/policies/conditionalAccessPolicies/{conditionalAccessPolicyId}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.conditionalAccessPolicy",
    "id": "a171f761-f761-a171-61f7-71a161f771a1",
    "createdDateTime": "String (timestamp)",
    "modifiedDateTime": "String (timestamp)",
    "displayName": "String",
    "description": "String",
    "state": "String",
    "conditions": {
      "@odata.type": "microsoft.graph.conditionalAccessConditionSet"
    },
    "grantControls": {
      "@odata.type": "microsoft.graph.conditionalAccessGrantControls"
    },
    "sessionControls": {
      "@odata.type": "microsoft.graph.conditionalAccessSessionControls"
    }
  }
}
```


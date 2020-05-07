---
title: "List messageRules"
description: "Get the messageRules from the messageRules navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List messageRules

Namespace: microsoft.graph

Get the messageRules from the messageRules navigation property.

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
GET /users/{usersId}/mailFolders/{mailFolderId}/messageRules
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

If successful, this method returns a `200 OK` response code and a collection of [messageRule](../resources/messagerule.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_messagerule"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mailFolders/{mailFolderId}/messageRules
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.messagerule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.messageRule",
      "id": "205d555c-555c-205d-5c55-5d205c555d20",
      "displayName": "String",
      "sequence": "Integer",
      "conditions": {
        "@odata.type": "microsoft.graph.messageRulePredicates"
      },
      "actions": {
        "@odata.type": "microsoft.graph.messageRuleActions"
      },
      "exceptions": {
        "@odata.type": "microsoft.graph.messageRulePredicates"
      },
      "isEnabled": "Boolean",
      "hasError": "Boolean",
      "isReadOnly": "Boolean"
    }
  ]
}
```


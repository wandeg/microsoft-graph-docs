---
title: "Create messageRules"
description: "Create a new messageRules object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create messageRules

Namespace: microsoft.graph

Create a new messageRules object.

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
POST /users/{usersId}/mailFolders/{mailFolderId}/messageRules
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [messageRule](../resources/messagerule.md) object.

The following table shows the properties that are required when you create the [messageRule](../resources/messagerule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|conditions|[messageRulePredicates](../resources/messagerulepredicates.md)|**TODO: Add Description**|
|actions|[messageRuleActions](../resources/messageruleactions.md)|**TODO: Add Description**|
|exceptions|[messageRulePredicates](../resources/messagerulepredicates.md)|**TODO: Add Description**|
|isEnabled|Boolean|**TODO: Add Description**|
|hasError|Boolean|**TODO: Add Description**|
|isReadOnly|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [messageRule](../resources/messagerule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_messagerule_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/mailFolders/{mailFolderId}/messageRules
Content-Type: application/json
Content-length: 437

{
  "@odata.type": "#microsoft.graph.messageRule",
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
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.messagerule"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.messageRule",
  "id": "f11b4b7b-4b7b-f11b-7b4b-1bf17b4b1bf1",
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
```


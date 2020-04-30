---
title: "Create groupLifecyclePolicies"
description: "Create a new groupLifecyclePolicies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create groupLifecyclePolicies

Namespace: microsoft.graph

Create a new groupLifecyclePolicies object.

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
POST ** Collection URI for microsoft.graph.groupLifecyclePolicy not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.

The following table shows the properties that are required when you create the [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|groupLifetimeInDays|Int32|**TODO: Add Description**|
|managedGroupTypes|String|**TODO: Add Description**|
|alternateNotificationEmails|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and a [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_grouplifecyclepolicies"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.groupLifecyclePolicy not found
Content-Type: application/json
Content-length: 177

{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "groupLifetimeInDays": "Integer",
  "managedGroupTypes": "String",
  "alternateNotificationEmails": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouplifecyclepolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.groupLifecyclePolicy",
  "id": "13959d80-9d80-1395-809d-9513809d9513",
  "groupLifetimeInDays": "Integer",
  "managedGroupTypes": "String",
  "alternateNotificationEmails": "String"
}
```


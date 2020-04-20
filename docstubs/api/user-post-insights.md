---
title: "Create insights"
description: "Create a new insights object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create insights

Namespace: microsoft.graph

Create a new insights object.

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
POST /me/insights
POST /users/{usersId}/insights
POST /invitations/{invitationsId}/invitedUser/insights
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [officeGraphInsights](../resources/officegraphinsights.md) object.

The following table shows the properties that are required when you create the [officeGraphInsights](../resources/officegraphinsights.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and an [officeGraphInsights](../resources/officegraphinsights.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_officegraphinsights_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/insights
Content-Type: application/json
Content-length: 61

{
  "@odata.type": "#microsoft.graph.officeGraphInsights"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.officegraphinsights"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.officeGraphInsights",
  "id": "650055e6-55e6-6500-e655-0065e6550065"
}
```


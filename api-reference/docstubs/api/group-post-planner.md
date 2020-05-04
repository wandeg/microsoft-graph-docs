---
title: "Create planner"
description: "Create a new planner object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create planner

Namespace: microsoft.graph

Create a new planner object.

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
POST /groups/{groupsId}/planner
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [plannerGroup](../resources/plannergroup.md) object.

The following table shows the properties that are required when you create the [plannerGroup](../resources/plannergroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response
If successful, this method returns a `201 Created` response code and a [plannerGroup](../resources/plannergroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannergroup_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/groups/{groupsId}/planner
Content-Type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.plannerGroup"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannergroup"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerGroup",
  "id": "2bca57fa-57fa-2bca-fa57-ca2bfa57ca2b"
}
```


---
title: "Create recentPlans"
description: "Create recentPlans by posting to the recentPlans collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create recentPlans

Namespace: microsoft.graph

Create recentPlans by posting to the recentPlans collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/planner/recentPlans/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [plannerPlan](../resources/plannerplan.md) object.

The following table shows the properties that are required when you create the [plannerPlan](../resources/plannerplan.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)||
|createdDateTime|DateTimeOffset||
|owner|String||
|title|String||
|contexts|[plannerPlanContextCollection](../resources/plannerplancontextcollection.md)||



## Response
If successful, this method returns a `201 Created` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/planner/recentPlans
Content-type: application/json
Content-length: 565

{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "owner": "Owner value",
  "title": "Title value",
  "contexts": {
    "@odata.type": "microsoft.graph.plannerPlanContextCollection"
  }
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerplan"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 673

{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "id": "6e4f2486-2486-6e4f-8624-4f6e86244f6e",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "2016-12-31T23:57:52.9071279+03:00",
  "owner": "Owner value",
  "title": "Title value",
  "contexts": {
    "@odata.type": "microsoft.graph.plannerPlanContextCollection"
  }
}
```


---
title: "Add plans"
description: "Add plans by posting to the plans collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add plans

Namespace: microsoft.graph

Add plans by posting to the plans collection.

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
POST /invitations/{invitationsId}/invitedUser/planner/plans/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [plannerPlan](../resources/plannerplan.md) object.

The following table shows the properties that are required when you create the [plannerPlan](../resources/plannerplan.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|
|title|String|**TODO: Add Description**|



## Response
If successful, this method returns a `204 No Content` response code and a [plannerPlan](../resources/plannerplan.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerplan_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/planner/plans/$ref
Content-Type: application/json
Content-length: 475

{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "owner": "Owner value",
  "title": "Title value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerplan"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.plannerPlan",
  "id": "edaafab4-fab4-edaa-b4fa-aaedb4faaaed",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "displayName": "Display Name value",
      "id": "Id value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  },
  "createdDateTime": "2017-01-01T00:02:24.9669049+03:00",
  "owner": "Owner value",
  "title": "Title value"
}
```


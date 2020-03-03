---
title: "List plannerPlans"
description: "List properties and relationships of the plannerPlan objects."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List plannerPlans

Namespace: microsoft.graph

List properties and relationships of the [plannerPlan](../resources/plannerplan.md) objects.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /planner/plans
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [plannerPlan](../resources/plannerplan.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_plannerplan"
}
-->
``` http
GET https://graph.microsoft.com/localtest/planner/plans
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.plannerplan)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 691

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.plannerPlan",
      "id": "e72c80e4-80e4-e72c-e480-2ce7e4802ce7",
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
      "createdDateTime": "2017-01-01T00:02:24.618735+03:00",
      "owner": "Owner value",
      "title": "Title value"
    }
  ]
}
```


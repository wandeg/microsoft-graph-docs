---
title: "List activityBasedTimeoutPolicies"
description: "Get the activityBasedTimeoutPolicies from the activityBasedTimeoutPolicies navigation property."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# List activityBasedTimeoutPolicies

Namespace: microsoft.graph

Get the activityBasedTimeoutPolicies from the activityBasedTimeoutPolicies navigation property.

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
GET /policies/activityBasedTimeoutPolicies
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.activitybasedtimeoutpolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.activityBasedTimeoutPolicy",
      "id": "bd53a6c0-a6c0-bd53-c0a6-53bdc0a653bd",
      "description": "Description value",
      "displayName": "Display Name value",
      "definition": [
        "Definition value"
      ],
      "isOrganizationDefault": true
    }
  ]
}
```


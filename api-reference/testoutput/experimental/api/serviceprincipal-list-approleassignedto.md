---
title: "List appRoleAssignedTo"
description: "Get the appRoleAssignments from the appRoleAssignedTo navigation property."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# List appRoleAssignedTo

Namespace: microsoft.graph

Get the appRoleAssignments from the appRoleAssignedTo navigation property.

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
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/localtest/servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.approleassignment)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 569

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appRoleAssignment",
      "id": "1f1a57b9-57b9-1f1a-b957-1a1fb9571a1f",
      "appRoleId": "69b07452-7452-69b0-5274-b0695274b069",
      "creationTimestamp": "2016-12-31T23:58:26.7160995+03:00",
      "principalDisplayName": "Principal Display Name value",
      "principalId": "b505019e-019e-b505-9e01-05b59e0105b5",
      "principalType": "Principal Type value",
      "resourceDisplayName": "Resource Display Name value",
      "resourceId": "2fe2697f-697f-2fe2-7f69-e22f7f69e22f"
    }
  ]
}
```


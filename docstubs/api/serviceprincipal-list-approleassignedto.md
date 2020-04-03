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

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}
-->
``` http
GET https://graph.microsoft.com/beta/servicePrincipals/{servicePrincipalsId}/appRoleAssignedTo
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
Content-Length: 568

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appRoleAssignment",
      "id": "3ca445ac-45ac-3ca4-ac45-a43cac45a43c",
      "appRoleId": "63373109-3109-6337-0931-376309313763",
      "creationTimestamp": "2016-12-31T23:56:55.872626+00:00",
      "principalDisplayName": "Principal Display Name value",
      "principalId": "3c0b18e9-18e9-3c0b-e918-0b3ce9180b3c",
      "principalType": "Principal Type value",
      "resourceDisplayName": "Resource Display Name value",
      "resourceId": "41c49f25-9f25-41c4-259f-c441259fc441"
    }
  ]
}
```


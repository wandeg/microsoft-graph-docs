---
title: "Get governanceResource"
description: "Read properties and relationships of the governanceResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get governanceResource

Namespace: microsoft.graph

Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.

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
GET /governanceResources/{governanceResourcesId}
GET /governanceResources/{governanceResourcesId}/parent
GET /governanceRoleSettings/{governanceRoleSettingsId}/resource
GET /governanceRoleDefinitions/{governanceRoleDefinitionsId}/resource
GET /governanceRoleAssignments/{governanceRoleAssignmentsId}/resource
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/parent
GET /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/resource
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/resource
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}/resource
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/roleSetting/resource
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/resource
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
If successful, this method returns a `200 OK` response code and [governanceResource](../resources/governanceresource.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governanceresource"
}
-->
``` http
GET https://graph.microsoft.com/beta/governanceResources/{governanceResourcesId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceResource"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 383

{
  "value": {
    "@odata.type": "#microsoft.graph.governanceResource",
    "id": "5681617e-617e-5681-7e61-81567e618156",
    "externalId": "External Id value",
    "type": "Type value",
    "displayName": "Display Name value",
    "status": "Status value",
    "registeredDateTime": "2016-12-31T23:56:57.760392+03:00",
    "registeredRoot": "Registered Root value"
  }
}
```


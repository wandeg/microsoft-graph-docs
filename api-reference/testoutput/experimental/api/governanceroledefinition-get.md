---
title: "Get governanceRoleDefinition"
description: "Read properties and relationships of the governanceRoleDefinition object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get governanceRoleDefinition

Namespace: microsoft.graph

Read properties and relationships of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.

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
GET /governanceRoleDefinitions/{governanceRoleDefinitionsId}
GET /governanceRoleSettings/{governanceRoleSettingsId}/roleDefinition
GET /governanceRoleAssignments/{governanceRoleAssignmentsId}/roleDefinition
GET /privilegedAccess/{privilegedAccessId}/roleDefinitions/{governanceRoleDefinitionId}
GET /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/roleDefinition
GET /governanceResources/{governanceResourcesId}/roleDefinitions/{governanceRoleDefinitionId}
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}/roleDefinition
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/roleSetting/roleDefinition
GET /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/roleDefinition
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [governanceRoleDefinition](../resources/governanceroledefinition.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_governanceroledefinition"
}
-->
``` http
GET https://graph.microsoft.com/localtest/governanceRoleDefinitions/{governanceRoleDefinitionsId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.governanceRoleDefinition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 300

{
  "value": {
    "@odata.type": "#microsoft.graph.governanceRoleDefinition",
    "id": "88a029d0-29d0-88a0-d029-a088d029a088",
    "resourceId": "Resource Id value",
    "externalId": "External Id value",
    "templateId": "Template Id value",
    "displayName": "Display Name value"
  }
}
```


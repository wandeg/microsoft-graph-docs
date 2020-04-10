---
title: "Delete governanceResource"
description: "Deletes a governanceResource."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Delete governanceResource

Namespace: microsoft.graph

Deletes a [governanceResource](../resources/governanceresource.md).

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
DELETE /governanceResources/{governanceResourcesId}
DELETE /governanceResources/{governanceResourcesId}/parent
DELETE /governanceRoleSettings/{governanceRoleSettingsId}/resource
DELETE /governanceRoleDefinitions/{governanceRoleDefinitionsId}/resource
DELETE /governanceRoleAssignments/{governanceRoleAssignmentsId}/resource
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/parent
DELETE /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/resource
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/resource
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}/resource
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/roleSetting/resource
DELETE /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/resource
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "delete_governanceresource"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/governanceResources/{governanceResourcesId}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


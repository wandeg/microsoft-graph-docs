---
title: "Update governanceResource"
description: "Update the properties of a governanceResource object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update governanceResource

Update the properties of a [governanceResource](../resources/governanceresource.md) object.

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
PATCH /governanceResources/{governanceResourcesId}
PATCH /governanceResources/{governanceResourcesId}/parent
PATCH /governanceRoleSettings/{governanceRoleSettingsId}/resource
PATCH /governanceRoleDefinitions/{governanceRoleDefinitionsId}/resource
PATCH /governanceRoleAssignments/{governanceRoleAssignmentsId}/resource
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/parent
PATCH /governanceRoleAssignmentRequests/{governanceRoleAssignmentRequestsId}/resource
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/resource
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignments/{governanceRoleAssignmentId}/resource
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleDefinitions/{governanceRoleDefinitionId}/roleSetting/resource
PATCH /privilegedAccess/{privilegedAccessId}/resources/{governanceResourceId}/roleAssignmentRequests/{governanceRoleAssignmentRequestId}/resource
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|

## Request body
In the request body, supply a JSON representation for the [governanceResource](../resources/governanceResource.md) object.

The following table shows the properties that are required when you create the [governanceResource](../resources/governanceresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|externalId|String||
|type|String||
|displayName|String||
|status|String||
|registeredDateTime|DateTimeOffset||
|registeredRoot|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [governanceResource](../resources/governanceresource.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_governanceresource"
}
-->
``` http
PATCH https://graph.microsoft.com/docs\api/governanceResources/{governanceResourcesId}
Content-type: application/json
Content-length: 300

{
  "@odata.type": "#microsoft.graph.governanceResource",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2017-01-01T00:00:03.0159289+03:00",
  "registeredRoot": "Registered Root value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "@odata.type": "#microsoft.graph.governanceResource",
  "id": "8fd0522d-522d-8fd0-2d52-d08f2d52d08f",
  "externalId": "External Id value",
  "type": "Type value",
  "displayName": "Display Name value",
  "status": "Status value",
  "registeredDateTime": "2017-01-01T00:00:03.0159289+03:00",
  "registeredRoot": "Registered Root value"
}
```


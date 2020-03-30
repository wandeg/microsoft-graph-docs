---
title: "Add accessPackageAssignmentResourceRoles"
description: "Add accessPackageAssignmentResourceRoles by posting to the accessPackageAssignmentResourceRoles collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageAssignmentResourceRoles

Namespace: microsoft.graph

Add accessPackageAssignmentResourceRoles by posting to the accessPackageAssignmentResourceRoles collection.

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
POST /accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentResourceRoles/$ref
POST /identityGovernance/entitlementManagement/accessPackageAssignments/{accessPackageAssignmentId}/accessPackageAssignmentResourceRoles/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|originId|String||
|originSystem|String||
|status|String||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentresourcerole_from_accesspackageassignmentresourceroles"
}
-->
``` http
POST https://graph.microsoft.com/beta/accessPackageAssignments/{accessPackageAssignmentsId}/accessPackageAssignmentResourceRoles
Content-type: application/json
Content-length: 182

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "status": "Status value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignmentresourcerole"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 231

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentResourceRole",
  "id": "fe880eb2-0eb2-fe88-b20e-88feb20e88fe",
  "originId": "Origin Id value",
  "originSystem": "Origin System value",
  "status": "Status value"
}
```


---
title: "Add accessPackageAssignmentPolicies"
description: "Add accessPackageAssignmentPolicies by posting to the accessPackageAssignmentPolicies collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add accessPackageAssignmentPolicies

Add accessPackageAssignmentPolicies by posting to the accessPackageAssignmentPolicies collection.

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
POST /accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies/$ref
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageAssignmentPolicies/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the accessPackageAssignmentPolicy object.

The following table shows the properties that are required when you create the accessPackageAssignmentPolicy.

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|userType|String||
|accessPackageId|String||
|displayName|String||
|description|String||
|isEnabled|Boolean||
|canExtend|Boolean||
|durationInDays|Int32||
|expirationDateTime|DateTimeOffset||
|createdBy|String||
|createdDateTime|DateTimeOffset||
|modifiedBy|String||
|modifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `201 Created` response code and a [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}
-->
``` http
POST https://graph.microsoft.com/docs\api/accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies
Content-type: application/json
Content-length: 437

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "userType": "User Type value",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isEnabled": true,
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2017-01-01T00:01:09.280378+03:00",
  "createdBy": "Created By value",
  "modifiedBy": "Modified By value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageassignmentpolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 605

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "4908a4f3-a4f3-4908-f3a4-0849f3a40849",
  "userType": "User Type value",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isEnabled": true,
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2017-01-01T00:01:09.280378+03:00",
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:00:46.1697867+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2017-01-01T00:03:12.7204145+03:00"
}
```


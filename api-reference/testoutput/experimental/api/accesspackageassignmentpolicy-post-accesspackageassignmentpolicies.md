---
title: "Create accessPackageAssignmentPolicy"
description: "Create a new accessPackageAssignmentPolicy object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create accessPackageAssignmentPolicy

Namespace: microsoft.graph

Create a new [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

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
POST /accessPackageAssignmentPolicies
POST /accessPackages/{accessPackagesId}/accessPackageAssignmentPolicies
POST /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
POST /identityGovernance/entitlementManagement/accessPackageCatalogs/{accessPackageCatalogId}/accessPackages/{accessPackageId}/accessPackageAssignmentPolicies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.

The following table shows the properties that are required when you create the [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md).

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

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_accesspackageassignmentpolicy_from_accesspackageassignmentpolicies"
}
-->
``` http
POST https://graph.microsoft.com/localtest/accessPackageAssignmentPolicies
Content-type: application/json
Content-length: 438

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "userType": "User Type value",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isEnabled": true,
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00",
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
Content-Length: 606

{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentPolicy",
  "id": "3c72b1ab-b1ab-3c72-abb1-723cabb1723c",
  "userType": "User Type value",
  "accessPackageId": "Access Package Id value",
  "displayName": "Display Name value",
  "description": "Description value",
  "isEnabled": true,
  "canExtend": true,
  "durationInDays": 14,
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00",
  "createdBy": "Created By value",
  "createdDateTime": "2017-01-01T00:02:14.7219499+03:00",
  "modifiedBy": "Modified By value",
  "modifiedDateTime": "2016-12-31T23:58:13.3996216+03:00"
}
```


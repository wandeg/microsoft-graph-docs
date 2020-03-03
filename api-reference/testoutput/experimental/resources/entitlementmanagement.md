---
title: "entitlementManagement resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# entitlementManagement resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get entitlementManagement](../api/entitlementmanagement-get.md)|[entitlementManagement](../resources/entitlementManagement.md)|Read properties and relationships of the [entitlementManagement](../resources/entitlementmanagement.md) object.|
|[Update entitlementManagement](../api/entitlementmanagement-update.md)|[entitlementManagement](../resources/entitlementManagement.md)|Update the properties of a [entitlementManagement](../resources/entitlementmanagement.md) object.|
|[List accessPackageCatalogs](../api/entitlementmanagement-list-accesspackagecatalogs.md)|[accessPackageCatalog](../resources/accessPackageCatalog.md) collection|Get the accessPackageCatalogs from the accessPackageCatalogs navigation property.|
|[Add accessPackageCatalogs](../api/entitlementmanagement-post-accesspackagecatalogs.md)|[accessPackageCatalog](../resources/accessPackageCatalog.md)|Add accessPackageCatalogs by posting to the accessPackageCatalogs collection.|
|[List accessPackageResources](../api/entitlementmanagement-list-accesspackageresources.md)|[accessPackageResource](../resources/accessPackageResource.md) collection|Get the accessPackageResources from the accessPackageResources navigation property.|
|[Add accessPackageResources](../api/entitlementmanagement-post-accesspackageresources.md)|[accessPackageResource](../resources/accessPackageResource.md)|Add accessPackageResources by posting to the accessPackageResources collection.|
|[List accessPackageResourceRequests](../api/entitlementmanagement-list-accesspackageresourcerequests.md)|[accessPackageResourceRequest](../resources/accessPackageResourceRequest.md) collection|Get the accessPackageResourceRequests from the accessPackageResourceRequests navigation property.|
|[Add accessPackageResourceRequests](../api/entitlementmanagement-post-accesspackageresourcerequests.md)|[accessPackageResourceRequest](../resources/accessPackageResourceRequest.md)|Add accessPackageResourceRequests by posting to the accessPackageResourceRequests collection.|
|[List accessPackageResourceRoleScopes](../api/entitlementmanagement-list-accesspackageresourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accessPackageResourceRoleScope.md) collection|Get the accessPackageResourceRoleScopes from the accessPackageResourceRoleScopes navigation property.|
|[Add accessPackageResourceRoleScopes](../api/entitlementmanagement-post-accesspackageresourcerolescopes.md)|[accessPackageResourceRoleScope](../resources/accessPackageResourceRoleScope.md)|Add accessPackageResourceRoleScopes by posting to the accessPackageResourceRoleScopes collection.|
|[List accessPackages](../api/entitlementmanagement-list-accesspackages.md)|[accessPackage](../resources/accessPackage.md) collection|Get the accessPackages from the accessPackages navigation property.|
|[Add accessPackages](../api/entitlementmanagement-post-accesspackages.md)|[accessPackage](../resources/accessPackage.md)|Add accessPackages by posting to the accessPackages collection.|
|[List accessPackageAssignmentPolicies](../api/entitlementmanagement-list-accesspackageassignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accessPackageAssignmentPolicy.md) collection|Get the accessPackageAssignmentPolicies from the accessPackageAssignmentPolicies navigation property.|
|[Add accessPackageAssignmentPolicies](../api/entitlementmanagement-post-accesspackageassignmentpolicies.md)|[accessPackageAssignmentPolicy](../resources/accessPackageAssignmentPolicy.md)|Add accessPackageAssignmentPolicies by posting to the accessPackageAssignmentPolicies collection.|
|[List accessPackageAssignments](../api/entitlementmanagement-list-accesspackageassignments.md)|[accessPackageAssignment](../resources/accessPackageAssignment.md) collection|Get the accessPackageAssignments from the accessPackageAssignments navigation property.|
|[Add accessPackageAssignments](../api/entitlementmanagement-post-accesspackageassignments.md)|[accessPackageAssignment](../resources/accessPackageAssignment.md)|Add accessPackageAssignments by posting to the accessPackageAssignments collection.|
|[List accessPackageAssignmentRequests](../api/entitlementmanagement-list-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md) collection|Get the accessPackageAssignmentRequests from the accessPackageAssignmentRequests navigation property.|
|[Add accessPackageAssignmentRequests](../api/entitlementmanagement-post-accesspackageassignmentrequests.md)|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md)|Add accessPackageAssignmentRequests by posting to the accessPackageAssignmentRequests collection.|
|[List accessPackageAssignmentResourceRoles](../api/entitlementmanagement-list-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md) collection|Get the accessPackageAssignmentResourceRoles from the accessPackageAssignmentResourceRoles navigation property.|
|[Add accessPackageAssignmentResourceRoles](../api/entitlementmanagement-post-accesspackageassignmentresourceroles.md)|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md)|Add accessPackageAssignmentResourceRoles by posting to the accessPackageAssignmentResourceRoles collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackageAssignmentPolicies|[accessPackageAssignmentPolicy](../resources/accessPackageAssignmentPolicy.md) collection||
|accessPackageAssignmentRequests|[accessPackageAssignmentRequest](../resources/accessPackageAssignmentRequest.md) collection||
|accessPackageAssignmentResourceRoles|[accessPackageAssignmentResourceRole](../resources/accessPackageAssignmentResourceRole.md) collection||
|accessPackageAssignments|[accessPackageAssignment](../resources/accessPackageAssignment.md) collection||
|accessPackageCatalogs|[accessPackageCatalog](../resources/accessPackageCatalog.md) collection||
|accessPackageResourceRequests|[accessPackageResourceRequest](../resources/accessPackageResourceRequest.md) collection||
|accessPackageResourceRoleScopes|[accessPackageResourceRoleScope](../resources/accessPackageResourceRoleScope.md) collection||
|accessPackageResources|[accessPackageResource](../resources/accessPackageResource.md) collection||
|accessPackages|[accessPackage](../resources/accessPackage.md) collection||

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagement",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagement",
  "id": "String (identifier)"
}
```


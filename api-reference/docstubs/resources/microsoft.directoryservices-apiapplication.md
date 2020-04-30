---
title: "apiApplication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# apiApplication resource type


Namespace: Microsoft.DirectoryServices

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptMappedClaims|Boolean|**TODO: Add Description**|
|knownClientApplications|Guid collection|**TODO: Add Description**|
|oauth2PermissionScopes|[permissionScope](../resources/microsoft.directoryservices-permissionscope.md) collection|**TODO: Add Description**|
|preAuthorizedApplications|[preAuthorizedApplication](../resources/microsoft.directoryservices-preauthorizedapplication.md) collection|**TODO: Add Description**|
|requestedAccessTokenVersion|Int32|**TODO: Add Description**|
|resourceSpecificApplicationPermissions|[resourceSpecificPermission](../resources/microsoft.directoryservices-resourcespecificpermission.md) collection|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "Microsoft.DirectoryServices.apiApplication"
}
-->
``` json
{
  "@odata.type": "#Microsoft.DirectoryServices.apiApplication",
  "acceptMappedClaims": true,
  "knownClientApplications": [
    "Guid"
  ],
  "preAuthorizedApplications": [
    {
      "@odata.type": "Microsoft.DirectoryServices.preAuthorizedApplication",
      "appId": "String",
      "permissionIds": [
        "String"
      ]
    }
  ],
  "requestedAccessTokenVersion": 1024,
  "oauth2PermissionScopes": [
    {
      "@odata.type": "Microsoft.DirectoryServices.permissionScope",
      "adminConsentDescription": "String",
      "adminConsentDisplayName": "String",
      "id": "Guid",
      "isEnabled": true,
      "origin": "String",
      "type": "String",
      "userConsentDescription": "String",
      "userConsentDisplayName": "String",
      "value": "String"
    }
  ],
  "resourceSpecificApplicationPermissions": [
    {
      "@odata.type": "Microsoft.DirectoryServices.resourceSpecificPermission",
      "description": "String",
      "displayName": "String"
    }
  ]
}
```


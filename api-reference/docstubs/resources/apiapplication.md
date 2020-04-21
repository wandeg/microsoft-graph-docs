---
title: "apiApplication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: resourcePageType
---

# apiApplication resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptMappedClaims|Boolean|**TODO: Add Description**|
|knownClientApplications|Guid collection|**TODO: Add Description**|
|oauth2PermissionScopes|[permissionScope](../resources/permissionscope.md) collection|**TODO: Add Description**|
|preAuthorizedApplications|[preAuthorizedApplication](../resources/preauthorizedapplication.md) collection|**TODO: Add Description**|
|requestedAccessTokenVersion|Int32|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.apiApplication",
  "acceptMappedClaims": true,
  "knownClientApplications": [
    "Guid"
  ],
  "preAuthorizedApplications": [
    {
      "@odata.type": "microsoft.graph.preAuthorizedApplication",
      "appId": "String",
      "delegatedPermissionIds": [
        "String"
      ]
    }
  ],
  "requestedAccessTokenVersion": 1024,
  "oauth2PermissionScopes": [
    {
      "@odata.type": "microsoft.graph.permissionScope",
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
  ]
}
```


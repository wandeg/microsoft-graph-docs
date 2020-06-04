---
title: "apiApplication resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
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
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.apiApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.apiApplication",
  "acceptMappedClaims": "Boolean",
  "knownClientApplications": [
    "Guid"
  ],
  "preAuthorizedApplications": [
    {
      "@odata.type": "microsoft.graph.preAuthorizedApplication"
    }
  ],
  "requestedAccessTokenVersion": "Integer",
  "oauth2PermissionScopes": [
    {
      "@odata.type": "microsoft.graph.permissionScope"
    }
  ]
}
```


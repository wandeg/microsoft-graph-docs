---
title: "auditActor resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# auditActor resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationDisplayName|String|**TODO: Add Description**|
|applicationId|String|**TODO: Add Description**|
|ipAddress|String|**TODO: Add Description**|
|servicePrincipalName|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|userPermissions|String collection|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|userRoleScopeTags|[roleScopeTagInfo](../resources/rolescopetaginfo.md) collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditActor"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditActor",
  "type": "String",
  "userPermissions": [
    "String"
  ],
  "applicationId": "String",
  "applicationDisplayName": "String",
  "userPrincipalName": "String",
  "servicePrincipalName": "String",
  "ipAddress": "String",
  "userId": "String",
  "userRoleScopeTags": [
    {
      "@odata.type": "microsoft.graph.roleScopeTagInfo"
    }
  ]
}
```


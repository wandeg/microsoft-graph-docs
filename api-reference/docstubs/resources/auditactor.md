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
|applicationDisplayName|String|Name of the Application.|
|applicationId|String|AAD Application Id.|
|ipAddress|String|IPAddress.|
|servicePrincipalName|String|Service Principal Name (SPN).|
|type|String|Actor Type.|
|userId|String|User Id.|
|userPermissions|String collection|List of user permissions when the audit was performed.|
|userPrincipalName|String|User Principal Name (UPN).|
|userRoleScopeTags|[roleScopeTagInfo](../resources/rolescopetaginfo.md) collection|List of user scope tags when the audit was performed.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
      "@odata.type": "microsoft.graph.roleScopeTagInfo",
      "displayName": "String",
      "roleScopeTagId": "String"
    }
  ]
}
```


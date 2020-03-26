---
title: "oAuth2PermissionGrant resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# oAuth2PermissionGrant resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List oAuth2PermissionGrants](../api/oauth2permissiongrant-list.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection|List properties and relationships of the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) objects.|
|[Get oAuth2PermissionGrant](../api/oauth2permissiongrant-get.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)|Read properties and relationships of the [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.|
|[Create oAuth2PermissionGrant](../api/oauth2permissiongrant-post-oauth2permissiongrants.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)|Create a new [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.|
|[Delete oAuth2PermissionGrant](../api/oauth2permissiongrant-delete.md)|None|Deletes a [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md).|
|[Update oAuth2PermissionGrant](../api/oauth2permissiongrant-update.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md)|Update the properties of a [oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) object.|
|[delta](../api/oauth2permissiongrant-delta.md)|[oAuth2PermissionGrant](../resources/oauth2permissiongrant.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|clientId|String||
|consentType|String||
|expiryTime|DateTimeOffset||
|id|String| Inherited from [entity](../resources/entity.md)|
|principalId|String||
|resourceId|String||
|scope|String||
|startTime|DateTimeOffset||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.oAuth2PermissionGrant",
  "id": "String (identifier)",
  "clientId": "String",
  "consentType": "String",
  "expiryTime": "String (timestamp)",
  "principalId": "String",
  "resourceId": "String",
  "scope": "String",
  "startTime": "String (timestamp)"
}
```


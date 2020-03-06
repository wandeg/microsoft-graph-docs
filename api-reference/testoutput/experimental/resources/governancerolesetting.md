---
title: "governanceRoleSetting resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# governanceRoleSetting resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List governanceRoleSettings](../api/governancerolesetting-list.md)|[governanceRoleSetting](../resources/governancerolesetting.md) collection|List properties and relationships of the [governanceRoleSetting](../resources/governancerolesetting.md) objects.|
|[Get governanceRoleSetting](../api/governancerolesetting-get.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Read properties and relationships of the [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[Create governanceRoleSetting](../api/governancerolesetting-post-governancerolesettings.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Create a new [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[Delete governanceRoleSetting](../api/governancerolesetting-delete.md)|None|Deletes a [governanceRoleSetting](../resources/governancerolesetting.md).|
|[Update governanceRoleSetting](../api/governancerolesetting-update.md)|[governanceRoleSetting](../resources/governancerolesetting.md)|Update the properties of a [governanceRoleSetting](../resources/governancerolesetting.md) object.|
|[Get governanceRoleDefinition](../api/governanceroledefinition-get.md)|[governanceRoleDefinition](../resources/governanceroledefinition.md)|Read properties and relationships of the [governanceRoleDefinition](../resources/governanceroledefinition.md) object.|
|[Get governanceResource](../api/governanceresource-get.md)|[governanceResource](../resources/governanceresource.md)|Read properties and relationships of the [governanceResource](../resources/governanceresource.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|adminEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||
|adminMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDefault|Boolean||
|lastUpdatedBy|String||
|lastUpdatedDateTime|DateTimeOffset||
|resourceId|String||
|roleDefinitionId|String||
|userEligibleSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||
|userMemberSettings|[governanceRuleSetting](../resources/governancerulesetting.md) collection||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|resource|[governanceResource](../resources/governanceresource.md)||
|roleDefinition|[governanceRoleDefinition](../resources/governanceroledefinition.md)||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.governanceRoleSetting",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.governanceRoleSetting",
  "id": "String (identifier)",
  "resourceId": "String",
  "roleDefinitionId": "String",
  "isDefault": true,
  "lastUpdatedDateTime": "String (timestamp)",
  "lastUpdatedBy": "String",
  "adminEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting",
      "ruleIdentifier": "String",
      "setting": "String"
    }
  ],
  "adminMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userEligibleSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ],
  "userMemberSettings": [
    {
      "@odata.type": "microsoft.graph.governanceRuleSetting"
    }
  ]
}
```


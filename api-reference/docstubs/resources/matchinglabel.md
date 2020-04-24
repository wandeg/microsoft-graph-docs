---
title: "matchingLabel resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# matchingLabel resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationMode|applicationMode|**TODO: Add Description**. Possible values are: `manual`, `automatic`, `recommended`.|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isEndpointProtectionEnabled|Boolean|**TODO: Add Description**|
|labelActions|[labelActionBase](../resources/labelactionbase.md) collection|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|policyTip|String|**TODO: Add Description**|
|priority|Int32|**TODO: Add Description**|
|toolTip|String|**TODO: Add Description**|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.matchingLabel"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.matchingLabel",
  "id": "String (identifier)",
  "name": "String",
  "displayName": "String",
  "description": "String",
  "toolTip": "String",
  "policyTip": "String",
  "isEndpointProtectionEnabled": true,
  "applicationMode": "String",
  "labelActions": [
    {
      "@odata.type": "microsoft.graph.encryptWithUserDefinedRights",
      "encryptWith": "String",
      "decryptionRightsManagementTemplateId": "String",
      "allowMailForwarding": true,
      "allowAdHocPermissions": true
    }
  ],
  "priority": 1024
}
```


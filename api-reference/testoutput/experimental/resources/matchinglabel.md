---
title: "matchingLabel resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# matchingLabel resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicationMode|Enumeration|. Possible values are: `manual`, `automatic`, `recommended`.|
|description|String||
|displayName|String||
|id|String||
|isEndpointProtectionEnabled|Boolean||
|labelActions|[labelActionBase](../resources/labelactionbase.md) collection||
|name|String||
|policyTip|String||
|priority|Int32||
|toolTip|String||

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


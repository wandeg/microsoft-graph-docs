---
title: "encryptWithUserDefinedRights resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# encryptWithUserDefinedRights resource type


Namespace: microsoft.graph




Inherits from [encryptContent](../resources/encryptcontent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowAdHocPermissions|Boolean||
|allowMailForwarding|Boolean||
|decryptionRightsManagementTemplateId|String||
|encryptWith|Enumeration| Inherited from [encryptContent](../resources/encryptcontent.md). Possible values are: `template`, `userDefinedRights`.|
|name|String| Inherited from [labelActionBase](../resources/labelactionbase.md)|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.encryptWithUserDefinedRights"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.encryptWithUserDefinedRights",
  "name": "String",
  "encryptWith": "String",
  "decryptionRightsManagementTemplateId": "String",
  "allowMailForwarding": true,
  "allowAdHocPermissions": true
}
```


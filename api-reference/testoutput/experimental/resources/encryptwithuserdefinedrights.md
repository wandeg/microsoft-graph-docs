---
title: "encryptWithUserDefinedRights resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# encryptWithUserDefinedRights resource type




Inherits from [encryptContent](../resources/encryptContent.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowAdHocPermissions|Boolean||
|allowMailForwarding|Boolean||
|decryptionRightsManagementTemplateId|String||
|encryptWith|Enumeration| Inherited from [encryptContent](../resources/encryptContent.md). Possible values are: `template`, `userDefinedRights`.|
|name|String| Inherited from [labelActionBase](../resources/labelActionBase.md)|

## Relationships
None

## JSON Representation
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


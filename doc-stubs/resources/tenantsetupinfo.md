---
title: "tenantSetupInfo resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# tenantSetupInfo resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List tenantSetupInfoes](../api/tenantsetupinfo-list.md)|[tenantSetupInfo](../resources/tenantsetupinfo.md) collection|Get a list of the [tenantSetupInfo](../resources/tenantsetupinfo.md) objects and their properties.|
|[Create tenantSetupInfo](../api/tenantsetupinfo-create.md)|[tenantSetupInfo](../resources/tenantsetupinfo.md)|Create a new [tenantSetupInfo](../resources/tenantsetupinfo.md) object.|
|[Get tenantSetupInfo](../api/tenantsetupinfo-get.md)|[tenantSetupInfo](../resources/tenantsetupinfo.md)|Read the properties and relationships of a [tenantSetupInfo](../resources/tenantsetupinfo.md) object.|
|[Update tenantSetupInfo](../api/tenantsetupinfo-update.md)|[tenantSetupInfo](../resources/tenantsetupinfo.md)|Update the properties of a [tenantSetupInfo](../resources/tenantsetupinfo.md) object.|
|[Delete tenantSetupInfo](../api/tenantsetupinfo-delete.md)|None|Deletes a [tenantSetupInfo](../resources/tenantsetupinfo.md) object.|
|[List defaultRolesSettings](../api/tenantsetupinfo-list-defaultrolessettings.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md) collection|Get the privilegedRoleSettings from the defaultRolesSettings navigation property.|
|[Add defaultRolesSettings](../api/tenantsetupinfo-post-defaultrolessettings.md)|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|Add defaultRolesSettings by posting to the defaultRolesSettings collection.|
|[Remove defaultRolesSettings](../api/tenantsetupinfo-delete-defaultrolessettings.md)|None|Remove a [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|firstTimeSetup|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|relevantRolesSettings|String collection|**TODO: Add Description**|
|setupStatus|setupStatus|**TODO: Add Description**. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|
|skipSetup|Boolean|**TODO: Add Description**|
|userRolesActions|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|defaultRolesSettings|[privilegedRoleSettings](../resources/privilegedrolesettings.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.tenantSetupInfo",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.tenantSetupInfo",
  "id": "String (identifier)",
  "userRolesActions": "String",
  "firstTimeSetup": "Boolean",
  "relevantRolesSettings": [
    "String"
  ],
  "skipSetup": "Boolean",
  "setupStatus": "String"
}
```


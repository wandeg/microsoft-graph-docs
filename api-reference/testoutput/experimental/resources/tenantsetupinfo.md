---
title: "tenantSetupInfo resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# tenantSetupInfo resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List tenantSetupInfos](../api/tenantsetupinfo-list.md)|[tenantSetupInfo](../resources/tenantSetupInfo.md) collection|List properties and relationships of the [tenantSetupInfo](../resources/tenantsetupinfo.md) objects.|
|[Get tenantSetupInfo](../api/tenantsetupinfo-get.md)|[tenantSetupInfo](../resources/tenantSetupInfo.md)|Read properties and relationships of the [tenantSetupInfo](../resources/tenantsetupinfo.md) object.|
|[Create tenantSetupInfo](../api/tenantsetupinfo-create.md)|[tenantSetupInfo](../resources/tenantSetupInfo.md)|Create a new [tenantSetupInfo](../resources/tenantsetupinfo.md) object.|
|[Delete tenantSetupInfo](../api/tenantsetupinfo-delete.md)|None|Deletes a [tenantSetupInfo](../resources/tenantsetupinfo.md).|
|[Update tenantSetupInfo](../api/tenantsetupinfo-update.md)|[tenantSetupInfo](../resources/tenantSetupInfo.md)|Update the properties of a [tenantSetupInfo](../resources/tenantsetupinfo.md) object.|
|[Get privilegedRoleSettings](../api/privilegedrolesettings-get.md)|[privilegedRoleSettings](../resources/privilegedRoleSettings.md)|Read properties and relationships of the [privilegedRoleSettings](../resources/privilegedrolesettings.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|firstTimeSetup|Boolean||
|id|String| Inherited from [entity](../resources/entity.md)|
|relevantRolesSettings|String collection||
|setupStatus|Enumeration|. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|
|skipSetup|Boolean||
|userRolesActions|String||

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|defaultRolesSettings|[privilegedRoleSettings](../resources/privilegedRoleSettings.md)||

## JSON Representation
Here is a JSON representation of the resource.
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
  "firstTimeSetup": true,
  "relevantRolesSettings": [
    "String"
  ],
  "skipSetup": true,
  "setupStatus": "String"
}
```


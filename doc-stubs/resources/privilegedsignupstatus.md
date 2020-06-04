---
title: "privilegedSignupStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# privilegedSignupStatus resource type

Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List privilegedSignupStatus](../api/privilegedsignupstatus-list.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md) collection|Get a list of the [privilegedSignupStatus](../resources/privilegedsignupstatus.md) objects and their properties.|
|[Create privilegedSignupStatus](../api/privilegedsignupstatus-post-privilegedsignupstatus.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)|Create a new [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.|
|[Get privilegedSignupStatus](../api/privilegedsignupstatus-get.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)|Read the properties and relationships of a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.|
|[Update privilegedSignupStatus](../api/privilegedsignupstatus-update.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)|Update the properties of a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.|
|[Delete privilegedSignupStatus](../api/privilegedsignupstatus-delete.md)|None|Deletes a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.|
|[signUp](../api/privilegedsignupstatus-signup.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)|**TODO: Add Description**|
|[isSignedUp](../api/privilegedsignupstatus-issignedup.md)|Boolean|**TODO: Add Description**|
|[canSignUp](../api/privilegedsignupstatus-cansignup.md)|Boolean|**TODO: Add Description**|
|[completeSetup](../api/privilegedsignupstatus-completesetup.md)|[roleSuccessStatistics](../resources/rolesuccessstatistics.md) collection|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isRegistered|Boolean|**TODO: Add Description**|
|status|setupStatus|**TODO: Add Description**. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.privilegedSignupStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.privilegedSignupStatus",
  "id": "String (identifier)",
  "isRegistered": "Boolean",
  "status": "String"
}
```


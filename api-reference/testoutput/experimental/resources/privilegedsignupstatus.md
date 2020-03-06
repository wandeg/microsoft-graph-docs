---
title: "privilegedSignupStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# privilegedSignupStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List privilegedSignupStatuses](../api/privilegedsignupstatus-list.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md) collection|List properties and relationships of the [privilegedSignupStatus](../resources/privilegedsignupstatus.md) objects.|
|[Get privilegedSignupStatus](../api/privilegedsignupstatus-get.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)|Read properties and relationships of the [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.|
|[Create privilegedSignupStatus](../api/privilegedsignupstatus-post-privilegedsignupstatus.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)|Create a new [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.|
|[Delete privilegedSignupStatus](../api/privilegedsignupstatus-delete.md)|None|Deletes a [privilegedSignupStatus](../resources/privilegedsignupstatus.md).|
|[Update privilegedSignupStatus](../api/privilegedsignupstatus-update.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)|Update the properties of a [privilegedSignupStatus](../resources/privilegedsignupstatus.md) object.|
|[signUp](../api/privilegedsignupstatus-signup.md)|[privilegedSignupStatus](../resources/privilegedsignupstatus.md)||
|[isSignedUp](../api/privilegedsignupstatus-issignedup.md)|Boolean||
|[canSignUp](../api/privilegedsignupstatus-cansignup.md)|Boolean||
|[completeSetup](../api/privilegedsignupstatus-completesetup.md)|[roleSuccessStatistics](../resources/rolesuccessstatistics.md) collection||

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|isRegistered|Boolean||
|status|Enumeration|. Possible values are: `unknown`, `notRegisteredYet`, `registeredSetupNotStarted`, `registeredSetupInProgress`, `registrationAndSetupCompleted`, `registrationFailed`, `registrationTimedOut`, `disabled`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
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
  "isRegistered": true,
  "status": "String"
}
```


---
title: "appConsentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# appConsentRequest resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get appConsentRequest](../api/appconsentrequest-get.md)|[appConsentRequest](../resources/appconsentrequest.md)|Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.|
|[Update appConsentRequest](../api/appconsentrequest-update.md)|[appConsentRequest](../resources/appconsentrequest.md)|Update the properties of an [appConsentRequest](../resources/appconsentrequest.md) object.|
|[List userConsentRequests](../api/appconsentrequest-list-userconsentrequests.md)|[userConsentRequest](../resources/userconsentrequest.md) collection|Get the userConsentRequests from the userConsentRequests navigation property.|
|[Create userConsentRequests](../api/appconsentrequest-post-userconsentrequests.md)|[userConsentRequest](../resources/userconsentrequest.md)|Create a new userConsentRequests object.|
|[Delete userConsentRequests](../api/appconsentrequest-delete-userconsentrequests.md)|None|Delete a [userConsentRequest](../resources/userconsentrequest.md) object.|
|[Update userConsentRequests](../api/appconsentrequest-update-userconsentrequests.md)|[userConsentRequest](../resources/userconsentrequest.md)|Update the properties of a userConsentRequests object.|
|[Get userConsentRequest](../api/userconsentrequest-get.md)|[userConsentRequest](../resources/userconsentrequest.md)|Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.|
|[List appConsentRequestsForApproval](../api/user-list-appconsentrequestsforapproval.md)|[appConsentRequest](../resources/appconsentrequest.md) collection|Get the appConsentRequests from the appConsentRequestsForApproval navigation property.|
|[Create appConsentRequestsForApproval](../api/user-post-appconsentrequestsforapproval.md)|[appConsentRequest](../resources/appconsentrequest.md)|Create a new appConsentRequestsForApproval object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String|**TODO: Add Description**|
|appId|String|**TODO: Add Description**|
|consentType|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|pendingScopes|[appConsentRequestScope](../resources/appconsentrequestscope.md) collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|userConsentRequests|[userConsentRequest](../resources/userconsentrequest.md) collection|**TODO: Add Description**|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentRequest",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "consentType": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```


---
title: "iosVppEBook resource type"
description: "A class containing the properties for iOS Vpp eBook."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosVppEBook resource type


Namespace: microsoft.graph

A class containing the properties for iOS Vpp eBook.


Inherits from [managedEBook](../resources/managedebook.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List iosVppEBooks](../api/iosvppebook-list.md)|[iosVppEBook](../resources/iosvppebook.md) collection|List properties and relationships of the [iosVppEBook](../resources/iosvppebook.md) objects.|
|[Get iosVppEBook](../api/iosvppebook-get.md)|[iosVppEBook](../resources/iosvppebook.md)|Read properties and relationships of the [iosVppEBook](../resources/iosvppebook.md) object.|
|[Create iosVppEBook](../api/iosvppebook-create.md)|[iosVppEBook](../resources/iosvppebook.md)|Create a new [iosVppEBook](../resources/iosvppebook.md) object.|
|[Delete iosVppEBook](../api/iosvppebook-delete.md)|None|Deletes a [iosVppEBook](../resources/iosvppebook.md).|
|[Update iosVppEBook](../api/iosvppebook-update.md)|[iosVppEBook](../resources/iosvppebook.md)|Update the properties of a [iosVppEBook](../resources/iosvppebook.md) object.|
|[assign](../api/iosvppebook-assign.md)|None||
|[List categories](../api/iosvppebook-list-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md) collection|Get the managedEBookCategories from the categories navigation property.|
|[Create categories](../api/iosvppebook-post-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Create categories by posting to the categories collection.|
|[List assignments](../api/iosvppebook-list-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md) collection|Get the managedEBookAssignments from the assignments navigation property.|
|[Add assignments](../api/iosvppebook-post-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Add assignments by posting to the assignments collection.|
|[Get eBookInstallSummary](../api/ebookinstallsummary-get.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Read properties and relationships of the [eBookInstallSummary](../resources/ebookinstallsummary.md) object.|
|[List deviceStates](../api/iosvppebook-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallStates from the deviceStates navigation property.|
|[Add deviceStates](../api/iosvppebook-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Add deviceStates by posting to the deviceStates collection.|
|[List userStateSummary](../api/iosvppebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|Get the userInstallStateSummaries from the userStateSummary navigation property.|
|[Add userStateSummary](../api/iosvppebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Add userStateSummary by posting to the userStateSummary collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|The Apple ID associated with Vpp token.|
|createdDateTime|DateTimeOffset|The date and time when the eBook file was created. Inherited from [managedEBook](../resources/managedebook.md)|
|description|String|Description. Inherited from [managedEBook](../resources/managedebook.md)|
|displayName|String|Name of the eBook. Inherited from [managedEBook](../resources/managedebook.md)|
|genres|String collection|Genres.|
|id|String| Inherited from [entity](../resources/entity.md)|
|informationUrl|String|The more information Url. Inherited from [managedEBook](../resources/managedebook.md)|
|language|String|Language.|
|largeCover|[mimeContent](../resources/intune-apps-mimecontent.md)|Book cover. Inherited from [managedEBook](../resources/managedebook.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time when the eBook was last modified. Inherited from [managedEBook](../resources/managedebook.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [managedEBook](../resources/managedebook.md)|
|publishedDateTime|DateTimeOffset|The date and time when the eBook was published. Inherited from [managedEBook](../resources/managedebook.md)|
|publisher|String|Publisher. Inherited from [managedEBook](../resources/managedebook.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|seller|String|Seller.|
|totalLicenseCount|Int32|Total license count.|
|usedLicenseCount|Int32|Used license count.|
|vppOrganizationName|String|The Vpp token's organization name.|
|vppTokenId|Guid|The Vpp token ID.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/managedebookassignment.md) collection|The list of assignments for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|
|categories|[managedEBookCategory](../resources/managedebookcategory.md) collection|The list of categories for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|
|deviceStates|[deviceInstallState](../resources/deviceinstallstate.md) collection|The list of installation states for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|
|installSummary|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Mobile App Install Summary. Inherited from [managedEBook](../resources/managedebook.md)|
|userStateSummary|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|The list of installation states for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook",
  "baseType": "microsoft.graph.managedEBook",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "publishedDateTime": "String (timestamp)",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "informationUrl": "String",
  "privacyInformationUrl": "String",
  "vppTokenId": "Guid",
  "appleId": "String",
  "vppOrganizationName": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "seller": "String",
  "totalLicenseCount": 1024,
  "usedLicenseCount": 1024,
  "roleScopeTagIds": [
    "String"
  ]
}
```


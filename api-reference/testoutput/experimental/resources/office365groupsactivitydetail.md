---
title: "office365GroupsActivityDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# office365GroupsActivityDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List office365GroupsActivityDetails](../api/office365groupsactivitydetail-list.md)|[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) collection|List properties and relationships of the [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) objects.|
|[Get office365GroupsActivityDetail](../api/office365groupsactivitydetail-get.md)|[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)|Read properties and relationships of the [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) object.|
|[Create office365GroupsActivityDetail](../api/office365groupsactivitydetail-create.md)|[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)|Create a new [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) object.|
|[Delete office365GroupsActivityDetail](../api/office365groupsactivitydetail-delete.md)|None|Deletes a [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md).|
|[Update office365GroupsActivityDetail](../api/office365groupsactivitydetail-update.md)|[office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md)|Update the properties of a [office365GroupsActivityDetail](../resources/office365groupsactivitydetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|exchangeMailboxStorageUsedInBytes|Int64||
|exchangeMailboxTotalItemCount|Int64||
|exchangeReceivedEmailCount|Int64||
|externalMemberCount|Int64||
|groupDisplayName|String||
|groupId|String||
|groupType|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean||
|lastActivityDate|Date||
|memberCount|Int64||
|ownerPrincipalName|String||
|reportPeriod|String||
|reportRefreshDate|Date||
|sharePointActiveFileCount|Int64||
|sharePointSiteStorageUsedInBytes|Int64||
|sharePointTotalFileCount|Int64||
|yammerLikedMessageCount|Int64||
|yammerPostedMessageCount|Int64||
|yammerReadMessageCount|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.office365GroupsActivityDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.office365GroupsActivityDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "groupId": "String",
  "groupDisplayName": "String",
  "isDeleted": true,
  "ownerPrincipalName": "String",
  "lastActivityDate": "Date",
  "groupType": "String",
  "memberCount": 1024,
  "externalMemberCount": 1024,
  "exchangeReceivedEmailCount": 1024,
  "sharePointActiveFileCount": 1024,
  "yammerPostedMessageCount": 1024,
  "yammerReadMessageCount": 1024,
  "yammerLikedMessageCount": 1024,
  "exchangeMailboxTotalItemCount": 1024,
  "exchangeMailboxStorageUsedInBytes": 1024,
  "sharePointTotalFileCount": 1024,
  "sharePointSiteStorageUsedInBytes": 1024,
  "reportPeriod": "String"
}
```


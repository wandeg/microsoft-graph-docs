---
title: "emailAppUsageUserDetail resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# emailAppUsageUserDetail resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailAppUsageUserDetails](../api/emailappusageuserdetail-list.md)|[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) collection|List properties and relationships of the [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) objects.|
|[Get emailAppUsageUserDetail](../api/emailappusageuserdetail-get.md)|[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)|Read properties and relationships of the [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) object.|
|[Create emailAppUsageUserDetail](../api/emailappusageuserdetail-create.md)|[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)|Create a new [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) object.|
|[Delete emailAppUsageUserDetail](../api/emailappusageuserdetail-delete.md)|None|Deletes a [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md).|
|[Update emailAppUsageUserDetail](../api/emailappusageuserdetail-update.md)|[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)|Update the properties of a [emailAppUsageUserDetail](../resources/emailappusageuserdetail.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deletedDate|Date||
|displayName|String||
|id|String| Inherited from [entity](../resources/entity.md)|
|imap4App|String collection||
|isDeleted|Boolean||
|lastActivityDate|Date||
|mailForMac|String collection||
|otherForMobile|String collection||
|outlookForMac|String collection||
|outlookForMobile|String collection||
|outlookForWeb|String collection||
|outlookForWindows|String collection||
|pop3App|String collection||
|reportPeriod|String||
|reportRefreshDate|Date||
|smtpApp|String collection||
|userPrincipalName|String||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAppUsageUserDetail",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "userPrincipalName": "String",
  "displayName": "String",
  "isDeleted": true,
  "deletedDate": "Date",
  "lastActivityDate": "Date",
  "mailForMac": [
    "String"
  ],
  "outlookForMac": [
    "String"
  ],
  "outlookForWindows": [
    "String"
  ],
  "outlookForMobile": [
    "String"
  ],
  "otherForMobile": [
    "String"
  ],
  "outlookForWeb": [
    "String"
  ],
  "pop3App": [
    "String"
  ],
  "imap4App": [
    "String"
  ],
  "smtpApp": [
    "String"
  ],
  "reportPeriod": "String"
}
```


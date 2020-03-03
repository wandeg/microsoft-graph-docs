---
title: "emailAppUsageUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
Namespace: microsoft.graph
---


# emailAppUsageUserCounts resource type




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailAppUsageUserCountses](../api/emailappusageusercounts-list.md)|[emailAppUsageUserCounts](../resources/emailAppUsageUserCounts.md) collection|List properties and relationships of the [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) objects.|
|[Get emailAppUsageUserCounts](../api/emailappusageusercounts-get.md)|[emailAppUsageUserCounts](../resources/emailAppUsageUserCounts.md)|Read properties and relationships of the [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object.|
|[Create emailAppUsageUserCounts](../api/emailappusageusercounts-create.md)|[emailAppUsageUserCounts](../resources/emailAppUsageUserCounts.md)|Create a new [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object.|
|[Delete emailAppUsageUserCounts](../api/emailappusageusercounts-delete.md)|None|Deletes a [emailAppUsageUserCounts](../resources/emailappusageusercounts.md).|
|[Update emailAppUsageUserCounts](../api/emailappusageusercounts-update.md)|[emailAppUsageUserCounts](../resources/emailAppUsageUserCounts.md)|Update the properties of a [emailAppUsageUserCounts](../resources/emailappusageusercounts.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|imap4App|Int64||
|mailForMac|Int64||
|otherForMobile|Int64||
|outlookForMac|Int64||
|outlookForMobile|Int64||
|outlookForWeb|Int64||
|outlookForWindows|Int64||
|pop3App|Int64||
|reportDate|Date||
|reportPeriod|String||
|reportRefreshDate|Date||
|smtpApp|Int64||

## Relationships
None

## JSON Representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAppUsageUserCounts",
  "id": "String (identifier)",
  "reportRefreshDate": "Date",
  "mailForMac": 1024,
  "outlookForMac": 1024,
  "outlookForWindows": 1024,
  "outlookForMobile": 1024,
  "otherForMobile": 1024,
  "outlookForWeb": 1024,
  "pop3App": 1024,
  "imap4App": 1024,
  "smtpApp": 1024,
  "reportDate": "Date",
  "reportPeriod": "String"
}
```


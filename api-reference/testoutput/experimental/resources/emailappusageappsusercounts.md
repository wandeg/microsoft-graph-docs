---
title: "emailAppUsageAppsUserCounts resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# emailAppUsageAppsUserCounts resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List emailAppUsageAppsUserCountses](../api/emailappusageappsusercounts-list.md)|[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) collection|List properties and relationships of the [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) objects.|
|[Get emailAppUsageAppsUserCounts](../api/emailappusageappsusercounts-get.md)|[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)|Read properties and relationships of the [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) object.|
|[Create emailAppUsageAppsUserCounts](../api/emailappusageappsusercounts-create.md)|[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)|Create a new [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) object.|
|[Delete emailAppUsageAppsUserCounts](../api/emailappusageappsusercounts-delete.md)|None|Deletes a [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md).|
|[Update emailAppUsageAppsUserCounts](../api/emailappusageappsusercounts-update.md)|[emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md)|Update the properties of a [emailAppUsageAppsUserCounts](../resources/emailappusageappsusercounts.md) object.|

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
  "@odata.type": "microsoft.graph.emailAppUsageAppsUserCounts",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailAppUsageAppsUserCounts",
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
  "reportPeriod": "String"
}
```


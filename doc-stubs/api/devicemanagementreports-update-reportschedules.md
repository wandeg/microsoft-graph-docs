---
title: "Update reportSchedules"
description: "Update the properties of a reportSchedules object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update reportSchedules

Namespace: microsoft.graph

Update the properties of a reportSchedules object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|reportScheduleName|String|**TODO: Add Description**|
|subject|String|**TODO: Add Description**|
|emails|String collection|**TODO: Add Description**|
|recurrence|deviceManagementScheduledReportRecurrence|**TODO: Add Description**. Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|reportName|String|**TODO: Add Description**|
|filter|String|**TODO: Add Description**|
|select|String collection|**TODO: Add Description**|
|orderBy|String collection|**TODO: Add Description**|
|format|deviceManagementReportFileFormat|**TODO: Add Description**. Possible values are: `csv`, `pdf`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_reportschedules"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
Content-Type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "reportScheduleName": "String",
  "subject": "String",
  "emails": [
    "String"
  ],
  "recurrence": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "userId": "String",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "9107fee1-fee1-9107-e1fe-0791e1fe0791",
  "reportScheduleName": "String",
  "subject": "String",
  "emails": [
    "String"
  ],
  "recurrence": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "userId": "String",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String"
}
```


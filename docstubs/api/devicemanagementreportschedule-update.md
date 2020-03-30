---
title: "Update deviceManagementReportSchedule"
description: "Update the properties of a deviceManagementReportSchedule object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementReportSchedule

Namespace: microsoft.graph

Update the properties of a [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object.

The following table shows the properties that are required when you create the [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportScheduleName|String||
|subject|String||
|emails|String collection||
|recurrence|Enumeration| Possible values are: `none`, `daily`, `weekly`, `monthly`.|
|startDateTime|DateTimeOffset||
|endDateTime|DateTimeOffset||
|userId|String||
|reportName|String||
|filter|String||
|select|String collection||
|orderBy|String collection||
|format|Enumeration| Possible values are: `csv`, `pdf`.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementreportschedule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules/{deviceManagementReportScheduleId}
Content-type: application/json
Content-length: 543

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "String",
  "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
  "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "String"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 592

{
  "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
  "id": "fd905f8c-5f8c-fd90-8c5f-90fd8c5f90fd",
  "reportScheduleName": "Report Schedule Name value",
  "subject": "Subject value",
  "emails": [
    "Emails value"
  ],
  "recurrence": "String",
  "startDateTime": "2017-01-01T00:01:00.4985153+03:00",
  "endDateTime": "2017-01-01T00:01:31.3007329+03:00",
  "userId": "User Id value",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "format": "String"
}
```


---
title: "List reportSchedules"
description: "Get the deviceManagementReportSchedules from the reportSchedules navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List reportSchedules

Namespace: microsoft.graph

Get the deviceManagementReportSchedules from the reportSchedules navigation property.

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
GET /deviceManagement/reports/reportSchedules
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [deviceManagementReportSchedule](../resources/devicemanagementreportschedule.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementreportschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.devicemanagementreportschedule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```


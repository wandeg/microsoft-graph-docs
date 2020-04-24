---
title: "Create exportJobs"
description: "Create a new exportJobs object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create exportJobs

Namespace: microsoft.graph

Create a new exportJobs object.

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
POST /deviceManagement/reports/exportJobs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.

The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/devicemanagementexportjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|reportName|String|Name of the report|
|filter|String|Filters applied on the report|
|select|String collection|Columns selected from the report|
|format|deviceManagementReportFileFormat|Format of the exported report. Possible values are: `csv`, `pdf`.|
|snapshotId|String|A snapshot is an identifiable subset of the dataset represented by the ReportName. A sessionId or CachedReportConfiguration id can be used here. If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId. Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.|
|status|deviceManagementReportStatus|Status of the export job. Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String|Temporary location of the exported report|
|requestDateTime|DateTimeOffset|Time that the exported report was requested|
|expirationDateTime|DateTimeOffset|Time that the exported report expires|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementexportjob_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs
Content-Type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "String",
  "snapshotId": "Snapshot Id value",
  "status": "String",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:02:26.8557697+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementexportjob"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "593eb888-b888-593e-88b8-3e5988b83e59",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "String",
  "snapshotId": "Snapshot Id value",
  "status": "String",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:02:26.8557697+03:00",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00"
}
```


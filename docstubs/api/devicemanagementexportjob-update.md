---
title: "Update deviceManagementExportJob"
description: "Update the properties of a deviceManagementExportJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementExportJob

Namespace: microsoft.graph

Update the properties of a [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.

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
PATCH /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.

The following table shows the properties that are required when you create the [deviceManagementExportJob](../resources/devicemanagementexportjob.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportName|String||
|filter|String||
|select|String collection||
|format|Enumeration| Possible values are: `csv`, `pdf`.|
|snapshotId|String||
|status|Enumeration| Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|url|String||
|requestDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementexportjob"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
Content-type: application/json
Content-length: 403

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
  "requestDateTime": "2017-01-01T00:01:52.0217957+00:00",
  "expirationDateTime": "2016-12-31T23:58:53.1230242+00:00"
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
Content-Length: 452

{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "c6ca8360-8360-c6ca-6083-cac66083cac6",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "format": "String",
  "snapshotId": "Snapshot Id value",
  "status": "String",
  "url": "Url value",
  "requestDateTime": "2017-01-01T00:01:52.0217957+00:00",
  "expirationDateTime": "2016-12-31T23:58:53.1230242+00:00"
}
```


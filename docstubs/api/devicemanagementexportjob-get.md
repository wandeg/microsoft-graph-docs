---
title: "Get deviceManagementExportJob"
description: "Read properties and relationships of the deviceManagementExportJob object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementExportJob

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object.

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
GET /deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and [deviceManagementExportJob](../resources/devicemanagementexportjob.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementexportjob"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/exportJobs/{deviceManagementExportJobId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementExportJob"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 497

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementExportJob",
    "id": "91c72f1f-2f1f-91c7-1f2f-c7911f2fc791",
    "reportName": "Report Name value",
    "filter": "Filter value",
    "select": [
      "Select value"
    ],
    "format": "String",
    "snapshotId": "Snapshot Id value",
    "status": "String",
    "url": "Url value",
    "requestDateTime": "2017-01-01T00:00:18.1623191+03:00",
    "expirationDateTime": "2016-12-31T23:58:48.8634396+03:00"
  }
}
```


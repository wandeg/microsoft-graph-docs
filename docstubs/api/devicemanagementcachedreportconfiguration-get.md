---
title: "Get deviceManagementCachedReportConfiguration"
description: "Read properties and relationships of the deviceManagementCachedReportConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Get deviceManagementCachedReportConfiguration

Namespace: microsoft.graph

Read properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.

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
GET /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
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
If successful, this method returns a `200 OK` response code and [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "get_devicemanagementcachedreportconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementCachedReportConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 477

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
    "id": "1610c552-c552-1610-52c5-101652c51016",
    "reportName": "Report Name value",
    "filter": "Filter value",
    "select": [
      "Select value"
    ],
    "orderBy": [
      "Order By value"
    ],
    "status": "String",
    "lastRefreshDateTime": "2016-12-31T23:58:40.4688791+00:00",
    "expirationDateTime": "2016-12-31T23:57:47.0232285+00:00"
  }
}
```


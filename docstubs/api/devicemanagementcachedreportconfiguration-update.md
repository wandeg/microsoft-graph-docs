---
title: "Update deviceManagementCachedReportConfiguration"
description: "Update the properties of a deviceManagementCachedReportConfiguration object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementCachedReportConfiguration

Namespace: microsoft.graph

Update the properties of a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.

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
PATCH /deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.

The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportName|String||
|filter|String||
|select|String collection||
|orderBy|String collection||
|status|Enumeration| Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|lastRefreshDateTime|DateTimeOffset||
|expirationDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementcachedreportconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations/{deviceManagementCachedReportConfigurationId}
Content-type: application/json
Content-length: 383

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
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
Content-Length: 432

{
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
```


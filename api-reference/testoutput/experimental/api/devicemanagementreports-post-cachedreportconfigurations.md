---
title: "Add cachedReportConfigurations"
description: "Add cachedReportConfigurations by posting to the cachedReportConfigurations collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add cachedReportConfigurations

Namespace: microsoft.graph

Add cachedReportConfigurations by posting to the cachedReportConfigurations collection.

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
POST /deviceManagement/reports/cachedReportConfigurations/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object.

The following table shows the properties that are required when you create the [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|reportName|String|Name of the report|
|filter|String|Filters applied on report creation.|
|select|String collection|Columns selected from the report|
|orderBy|String collection|Ordering of columns in the report|
|status|Enumeration|Status of the cached report. Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.|
|lastRefreshDateTime|DateTimeOffset|Time that the cached report was last refreshed|
|expirationDateTime|DateTimeOffset|Time that the cached report expires|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementCachedReportConfiguration](../resources/devicemanagementcachedreportconfiguration.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementcachedreportconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/deviceManagement/reports/cachedReportConfigurations
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
  "lastRefreshDateTime": "2017-01-01T00:02:06.2859776+03:00",
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementcachedreportconfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 432

{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "14e13bf7-3bf7-14e1-f73b-e114f73be114",
  "reportName": "Report Name value",
  "filter": "Filter value",
  "select": [
    "Select value"
  ],
  "orderBy": [
    "Order By value"
  ],
  "status": "String",
  "lastRefreshDateTime": "2017-01-01T00:02:06.2859776+03:00",
  "expirationDateTime": "2017-01-01T00:01:27.2282595+03:00"
}
```


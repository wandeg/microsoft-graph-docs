---
title: "reportRoot: getOverallPrintUsageSummary"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# getOverallPrintUsageSummary

Namespace: microsoft.graph

**TODO: Add Description**

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
GET /print/reports/getOverallPrintUsageSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|periodStart|DateTimeOffset|**TODO: Add Description**|
|periodEnd|DateTimeOffset|**TODO: Add Description**|
|topListsSize|Int32|**TODO: Add Description**|



## Response
If successful, this function returns a `200 OK` response code and a [overallPrintUsageSummary](../resources/overallprintusagesummary.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getoverallprintusagesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/reports/getOverallPrintUsageSummary(periodStart=01/01/2017 00:01:32 +03:00,periodEnd=31/12/2016 23:58:30 +03:00,topListsSize=12)
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.overallprintusagesummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "microsoft.graph.overallPrintUsageSummary"
    }
  ]
}
```


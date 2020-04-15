---
title: "Update reportRoot"
description: "Update the properties of a reportRoot object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update reportRoot

Namespace: Microsoft.AAD.Reporting

Update the properties of a [reportRoot](../resources/microsoft.aad.reporting-reportroot.md) object.

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
PATCH /reports
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [reportRoot](../resources/microsoft.aad.reporting-reportroot.md) object.

The following table shows the properties that are required when you create the [reportRoot](../resources/microsoft.aad.reporting-reportroot.md).

|Property|Type|Description|
|:---|:---|:---|



## Response
If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/microsoft.aad.reporting-reportroot.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_reportroot"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/reports
Content-type: application/json
Content-length: 60

{
  "@odata.type": "#Microsoft.AAD.Reporting.reportRoot"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 60

{
  "@odata.type": "#Microsoft.AAD.Reporting.reportRoot"
}
```


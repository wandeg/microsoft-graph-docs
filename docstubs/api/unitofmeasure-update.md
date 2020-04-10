---
title: "Update unitOfMeasure"
description: "Update the properties of a unitOfMeasure object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update unitOfMeasure

Namespace: microsoft.graph

Update the properties of a [unitOfMeasure](../resources/unitofmeasure.md) object.

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
PATCH /financials/companies/{companyId}/unitsOfMeasure/{unitOfMeasureId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [unitOfMeasure](../resources/unitofmeasure.md) object.

The following table shows the properties that are required when you create the [unitOfMeasure](../resources/unitofmeasure.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|code|String||
|displayName|String||
|internationalStandardCode|String||
|lastModifiedDateTime|DateTimeOffset||



## Response
If successful, this method returns a `200 OK` response code and an updated [unitOfMeasure](../resources/unitofmeasure.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_unitofmeasure"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/unitsOfMeasure/{unitOfMeasureId}
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.unitOfMeasure",
  "code": "Code value",
  "displayName": "Display Name value",
  "internationalStandardCode": "International Standard Code value"
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
Content-Length: 302

{
  "@odata.type": "#microsoft.graph.unitOfMeasure",
  "id": "0d3bc986-c986-0d3b-86c9-3b0d86c93b0d",
  "code": "Code value",
  "displayName": "Display Name value",
  "internationalStandardCode": "International Standard Code value",
  "lastModifiedDateTime": "2016-12-31T23:58:51.0089696+00:00"
}
```


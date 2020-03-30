---
title: "Add unitsOfMeasure"
description: "Add unitsOfMeasure by posting to the unitsOfMeasure collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add unitsOfMeasure

Namespace: microsoft.graph

Add unitsOfMeasure by posting to the unitsOfMeasure collection.

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
POST /financials/companies/{companyId}/unitsOfMeasure/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

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
If successful, this method returns a `201 Created` response code and a [unitOfMeasure](../resources/unitofmeasure.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_unitofmeasure_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/unitsOfMeasure
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unitofmeasure"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 302

{
  "@odata.type": "#microsoft.graph.unitOfMeasure",
  "id": "6a75ca2b-ca2b-6a75-2bca-756a2bca756a",
  "code": "Code value",
  "displayName": "Display Name value",
  "internationalStandardCode": "International Standard Code value",
  "lastModifiedDateTime": "2016-12-31T23:59:45.9968839+03:00"
}
```


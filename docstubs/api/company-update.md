---
title: "Update company"
description: "Update the properties of a company object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update company

Namespace: microsoft.graph

Update the properties of a [company](../resources/company.md) object.

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
PATCH /financials/companies/{companyId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [company](../resources/company.md) object.

The following table shows the properties that are required when you create the [company](../resources/company.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|systemVersion|String||
|name|String||
|displayName|String||
|businessProfileId|String||



## Response
If successful, this method returns a `200 OK` response code and an updated [company](../resources/company.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_company"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.company",
  "systemVersion": "System Version value",
  "name": "Name value",
  "displayName": "Display Name value",
  "businessProfileId": "Business Profile Id value"
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
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.company",
  "id": "1fcc3dfb-3dfb-1fcc-fb3d-cc1ffb3dcc1f",
  "systemVersion": "System Version value",
  "name": "Name value",
  "displayName": "Display Name value",
  "businessProfileId": "Business Profile Id value"
}
```


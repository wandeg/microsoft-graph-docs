---
title: "Create company"
description: "Create a new company object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create company

Namespace: microsoft.graph

Create a new [company](../resources/company.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP Request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /financials/companies
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

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
If successful, this method returns a `201 Created` response code and a [company](../resources/company.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_company_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/financials/companies
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
  "truncated": true,
  "@odata.type": "microsoft.graph.company"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.company",
  "id": "deae77e1-77e1-deae-e177-aedee177aede",
  "systemVersion": "System Version value",
  "name": "Name value",
  "displayName": "Display Name value",
  "businessProfileId": "Business Profile Id value"
}
```


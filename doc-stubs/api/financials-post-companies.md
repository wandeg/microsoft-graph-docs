---
title: "Create companies"
description: "Create a new companies object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create companies

Namespace: microsoft.graph

Create a new companies object.

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
POST /financials/companies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [company](../resources/company.md) object.

The following table shows the properties that are required when you create the [company](../resources/company.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|systemVersion|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|businessProfileId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [company](../resources/company.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_company_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies
Content-Type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.company",
  "systemVersion": "String",
  "name": "String",
  "displayName": "String",
  "businessProfileId": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.company"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.company",
  "id": "2109c60c-c60c-2109-0cc6-09210cc60921",
  "systemVersion": "String",
  "name": "String",
  "displayName": "String",
  "businessProfileId": "String"
}
```


---
title: "Update cases"
description: "Update the properties of a cases object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update cases

Namespace: microsoft.graph

Update the properties of a cases object.

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
PATCH ** Collection URI for microsoft.compliance.ediscovery.contract.ediscoveryCase not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [ediscoveryCase](../resources/ediscoverycase.md) object.

The following table shows the properties that are required when you create the [ediscoveryCase](../resources/ediscoverycase.md).

|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|lastModifiedBy|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|caseStatus|**TODO: Add Description**. Possible values are: `unknown`, `active`, `pendingDelete`, `closing`, `closed`, `closedWithError`.|
|closedBy|String|**TODO: Add Description**|
|closedDateTime|DateTimeOffset|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_cases"
}
-->
``` http
PATCH https://graph.microsoft.com/beta** Collection URI for microsoft.compliance.ediscovery.contract.ediscoveryCase not found
Content-Type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.compliance.ediscovery.contract.ediscoveryCase",
  "description": "String",
  "createdBy": "String",
  "status": "String",
  "closedBy": "String",
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "displayName": "String"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "@odata.type": "#microsoft.compliance.ediscovery.contract.ediscoveryCase",
  "description": "String",
  "createdBy": "String",
  "lastModifiedBy": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "closedBy": "String",
  "closedDateTime": "String (timestamp)",
  "externalId": "String",
  "id": "61168e8c-8e8c-6116-8c8e-16618c8e1661",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```


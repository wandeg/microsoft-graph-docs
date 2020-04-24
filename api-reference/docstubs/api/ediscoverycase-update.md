---
title: "Update ediscoveryCase"
description: "Update the properties of an ediscoveryCase object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update ediscoveryCase

Namespace: microsoft.graph

Update the properties of an [ediscoveryCase](../resources/ediscoverycase.md) object.

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
PATCH /cases/{casesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [ediscoveryCase](../resources/ediscoverycase.md) object.

The following table shows the properties that are required when you create the [ediscoveryCase](../resources/ediscoverycase.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|description|String|**TODO: Add Description**|
|createdBy|String|**TODO: Add Description**|
|lastModifiedBy|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|caseStatus|**TODO: Add Description**. Possible values are: `unknown`, `active`, `pendingDelete`, `closing`, `closed`, `closedWithError`.|
|closedBy|String|**TODO: Add Description**|
|closedDateTime|DateTimeOffset|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_ediscoverycase"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/cases/{casesId}
Content-Type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "Description value",
  "createdBy": "Created By value",
  "status": "String",
  "closedBy": "Closed By value",
  "closedDateTime": "2016-12-31T23:58:06.1799456+03:00",
  "externalId": "External Id value",
  "displayName": "Display Name value"
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
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "id": "e2727eb4-7eb4-e272-b47e-72e2b47e72e2",
  "description": "Description value",
  "createdBy": "Created By value",
  "lastModifiedBy": "Last Modified By value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "status": "String",
  "closedBy": "Closed By value",
  "closedDateTime": "2016-12-31T23:58:06.1799456+03:00",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00"
}
```


---
title: "Create cases"
description: "Create a new cases object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create cases

Namespace: microsoft.graph

Create a new cases object.

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
POST /compliance/ediscovery/cases
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation for the [ediscoveryCase](../resources/ediscoverycase.md) object.

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
If successful, this method returns a `201 Created` response code and an [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_ediscoverycase_from_cases"
}
-->
``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-Type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "Description value",
  "createdBy": "Created By value",
  "status": "String",
  "closedBy": "Closed By value",
  "closedDateTime": "2016-12-31T23:57:03.2743031+00:00",
  "externalId": "External Id value",
  "displayName": "Display Name value"
}
```

### Response
Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscoverycase"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "id": "2a8e316b-316b-2a8e-6b31-8e2a6b318e2a",
  "description": "Description value",
  "createdBy": "Created By value",
  "lastModifiedBy": "Last Modified By value",
  "lastModifiedDateTime": "2017-01-01T00:00:09.5385853+00:00",
  "status": "String",
  "closedBy": "Closed By value",
  "closedDateTime": "2016-12-31T23:57:03.2743031+00:00",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "createdDateTime": "2016-12-31T23:57:19.8403601+00:00"
}
```


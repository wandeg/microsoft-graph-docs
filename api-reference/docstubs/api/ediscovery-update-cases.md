---
title: "Update cases"
description: "Update the properties of a cases object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
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
PATCH /compliance/ediscovery/cases
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

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
If successful, this method returns a `200 OK` response code and an updated [ediscoveryCase](../resources/ediscoverycase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_cases"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-Type: application/json
Content-length: 324

{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "description": "Description value",
  "createdBy": "Created By value",
  "status": "String",
  "closedBy": "Closed By value",
  "closedDateTime": "2016-12-31T23:59:21.4265692+00:00",
  "externalId": "External Id value",
  "displayName": "Display Name value"
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
{
  "@odata.type": "#microsoft.graph.ediscoveryCase",
  "id": "cb7ba1f3-a1f3-cb7b-f3a1-7bcbf3a17bcb",
  "description": "Description value",
  "createdBy": "Created By value",
  "lastModifiedBy": "Last Modified By value",
  "lastModifiedDateTime": "2016-12-31T23:58:12.0125666+00:00",
  "status": "String",
  "closedBy": "Closed By value",
  "closedDateTime": "2016-12-31T23:59:21.4265692+00:00",
  "externalId": "External Id value",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:14.13292+00:00"
}
```


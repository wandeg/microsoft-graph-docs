---
title: "Update dataPolicyOperation"
description: "Update the properties of a dataPolicyOperation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Update dataPolicyOperation

Namespace: microsoft.graph

Update the properties of a [dataPolicyOperation](../resources/datapolicyoperation.md) object.

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
PATCH /dataPolicyOperations/{dataPolicyOperationsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
In the request body, supply a JSON representation for the [dataPolicyOperation](../resources/datapolicyoperation.md) object.

The following table shows the properties that are required when you create the [dataPolicyOperation](../resources/datapolicyoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|status|dataPolicyOperationStatus|**TODO: Add Description**. Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|submittedDateTime|DateTimeOffset|**TODO: Add Description**|
|progress|Double|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_datapolicyoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataPolicyOperations/{dataPolicyOperationsId}
Content-Type: application/json
Content-length: 309

{
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "completedDateTime": "2017-01-01T00:01:00.1183272+00:00",
  "status": "String",
  "storageLocation": "Storage Location value",
  "userId": "User Id value",
  "submittedDateTime": "2017-01-01T00:03:27.8134844+00:00",
  "progress": "Double"
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
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "id": "84c3b1cd-b1cd-84c3-cdb1-c384cdb1c384",
  "completedDateTime": "2017-01-01T00:01:00.1183272+00:00",
  "status": "String",
  "storageLocation": "Storage Location value",
  "userId": "User Id value",
  "submittedDateTime": "2017-01-01T00:03:27.8134844+00:00",
  "progress": "Double"
}
```


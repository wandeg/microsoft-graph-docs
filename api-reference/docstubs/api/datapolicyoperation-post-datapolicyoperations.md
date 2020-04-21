---
title: "Create dataPolicyOperation"
description: "Create a new dataPolicyOperation object."
author: "**TODO: Provide Github Name**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod**"
doc_type: apiPageType
---

# Create dataPolicyOperation

Namespace: microsoft.graph

Create a new [dataPolicyOperation](../resources/datapolicyoperation.md) object.

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
POST /dataPolicyOperations
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `201 Created` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_datapolicyoperation_from_datapolicyoperations"
}
-->
``` http
POST https://graph.microsoft.com/beta/dataPolicyOperations
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
  "truncated": true,
  "@odata.type": "microsoft.graph.datapolicyoperation"
}
-->
``` http
HTTP/1.1 201 Created
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


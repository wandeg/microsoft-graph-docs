---
title: "Create dataPolicyOperation"
description: "Create a new dataPolicyOperation object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Create dataPolicyOperation

Namespace: microsoft.graph

Create a new [dataPolicyOperation](../resources/datapolicyoperation.md) object.

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
POST /dataPolicyOperations
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}|
|Content-Type|application/json|

## Request body
In the request body, supply a JSON representation for the [dataPolicyOperation](../resources/datapolicyoperation.md) object.

The following table shows the properties that are required when you create the [dataPolicyOperation](../resources/datapolicyoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|completedDateTime|DateTimeOffset||
|status|Enumeration|. Possible values are: `notStarted`, `running`, `complete`, `failed`, `unknownFutureValue`.|
|storageLocation|String||
|userId|String||
|submittedDateTime|DateTimeOffset||
|progress|Double||



## Response
If successful, this method returns a `201 Created` response code and a [dataPolicyOperation](../resources/datapolicyoperation.md) object in the response body.

## Example

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_datapolicyoperation_from_datapolicyoperations"
}
-->
``` http
POST https://graph.microsoft.com/localtest/dataPolicyOperations
Content-type: application/json
Content-length: 308

{
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "completedDateTime": "2017-01-01T00:03:28.7389204+03:00",
  "status": "String",
  "storageLocation": "Storage Location value",
  "userId": "User Id value",
  "submittedDateTime": "2017-01-01T00:01:26.640689+03:00",
  "progress": "Double"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.datapolicyoperation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 357

{
  "@odata.type": "#microsoft.graph.dataPolicyOperation",
  "id": "e9c5eb0d-eb0d-e9c5-0deb-c5e90debc5e9",
  "completedDateTime": "2017-01-01T00:03:28.7389204+03:00",
  "status": "String",
  "storageLocation": "Storage Location value",
  "userId": "User Id value",
  "submittedDateTime": "2017-01-01T00:01:26.640689+03:00",
  "progress": "Double"
}
```


---
title: "Update connectionOperation"
description: "Update the properties of a connectionOperation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update connectionOperation

Namespace: microsoft.graph

Update the properties of a [connectionOperation](../resources/connectionoperation.md) object.

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
PATCH /connections/{connectionsId}/operations/{connectionOperationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [connectionOperation](../resources/connectionoperation.md) object.

The following table shows the properties that are required when you create the [connectionOperation](../resources/connectionoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|status|connectionOperationStatus|**TODO: Add Description**. Possible values are: `unspecified`, `inprogress`, `completed`, `failed`.|
|error|[errorDetail](../resources/errordetail.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [connectionOperation](../resources/connectionoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_connectionoperation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/connections/{connectionsId}/operations/{connectionOperationId}
Content-Type: application/json
Content-length: 363

{
  "@odata.type": "#microsoft.graph.connectionOperation",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.errorDetail",
    "errorCode": "Error Code value",
    "message": "Message value",
    "details": [
      {
        "@odata.type": "microsoft.graph.innerErrorDetail",
        "source": "Source value"
      }
    ]
  }
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
  "@odata.type": "#microsoft.graph.connectionOperation",
  "id": "14334c87-4c87-1433-874c-3314874c3314",
  "status": "String",
  "error": {
    "@odata.type": "microsoft.graph.errorDetail",
    "errorCode": "Error Code value",
    "message": "Message value",
    "details": [
      {
        "@odata.type": "microsoft.graph.innerErrorDetail",
        "source": "Source value"
      }
    ]
  }
}
```


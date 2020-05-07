---
title: "Update jobs"
description: "Update the properties of a jobs object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update jobs

Namespace: microsoft.graph

Update the properties of a jobs object.

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
PATCH /dataClassification/jobs
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [jobResponseBase](../resources/jobresponsebase.md) object.

The following table shows the properties that are required when you create the [jobResponseBase](../resources/jobresponsebase.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|type|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|tenantId|String|**TODO: Add Description**|
|creationDateTime|DateTimeOffset|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|error|[classificationError](../resources/classificationerror.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [jobResponseBase](../resources/jobresponsebase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_jobs"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/dataClassification/jobs
Content-Type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "type": "String",
  "status": "String",
  "tenantId": "String",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
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
  "@odata.type": "#microsoft.graph.jobResponseBase",
  "id": "caad5ded-5ded-caad-ed5d-adcaed5dadca",
  "type": "String",
  "status": "String",
  "tenantId": "String",
  "creationDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "error": {
    "@odata.type": "microsoft.graph.classificationError"
  }
}
```


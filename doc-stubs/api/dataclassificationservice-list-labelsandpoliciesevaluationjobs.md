---
title: "List labelsAndPoliciesEvaluationJobs"
description: "Get the jobResponseBases from the labelsAndPoliciesEvaluationJobs navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List labelsAndPoliciesEvaluationJobs

Namespace: microsoft.graph

Get the jobResponseBases from the labelsAndPoliciesEvaluationJobs navigation property.

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
GET /dataClassification/labelsAndPoliciesEvaluationJobs
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [jobResponseBase](../resources/jobresponsebase.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_jobresponsebase"
}
-->
``` http
GET https://graph.microsoft.com/beta/dataClassification/labelsAndPoliciesEvaluationJobs
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.jobresponsebase)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
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
  ]
}
```


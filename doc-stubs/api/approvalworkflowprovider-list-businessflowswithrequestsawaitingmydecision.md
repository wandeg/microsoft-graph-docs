---
title: "List businessFlowsWithRequestsAwaitingMyDecision"
description: "Get the businessFlows from the businessFlowsWithRequestsAwaitingMyDecision navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List businessFlowsWithRequestsAwaitingMyDecision

Namespace: microsoft.graph

Get the businessFlows from the businessFlowsWithRequestsAwaitingMyDecision navigation property.

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
GET /approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlowsWithRequestsAwaitingMyDecision
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

If successful, this method returns a `200 OK` response code and a collection of [businessFlow](../resources/businessflow.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_businessflow"
}
-->
``` http
GET https://graph.microsoft.com/beta/approvalWorkflowProviders/{approvalWorkflowProvidersId}/businessFlowsWithRequestsAwaitingMyDecision
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.businessflow)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": [
    {
      "@odata.type": "#microsoft.graph.businessFlow",
      "id": "9d893a5d-3a5d-9d89-5d3a-899d5d3a899d",
      "displayName": "String",
      "description": "String",
      "deDuplicationId": "String",
      "schemaId": "String",
      "customData": "String",
      "recordVersion": "String",
      "policy": {
        "@odata.type": "microsoft.graph.governancePolicy"
      },
      "policyTemplateId": "String",
      "settings": {
        "@odata.type": "microsoft.graph.businessFlowSettings"
      }
    }
  ]
}
```


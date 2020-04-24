---
title: "Get threatAssessmentResult"
description: "Read the properties and relationships of a threatAssessmentResult object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get threatAssessmentResult

Namespace: microsoft.graph

Read the properties and relationships of a [threatAssessmentResult](../resources/threatassessmentresult.md) object.

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
GET /invitations/{invitationsId}/invitedUser/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/{threatAssessmentResultId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|

## Request body
Do not supply a request body for this method.

## Response
If successful, this method returns a `200 OK` response code and a [threatAssessmentResult](../resources/threatassessmentresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_threatassessmentresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results/{threatAssessmentResultId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatAssessmentResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.threatAssessmentResult",
    "id": "ff572c02-2c02-ff57-022c-57ff022c57ff",
    "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
    "resultType": "String",
    "message": "Message value"
  }
}
```


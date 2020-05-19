---
title: "Create results"
description: "Create a new results object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create results

Namespace: microsoft.graph

Create a new results object.

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
POST /informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [threatAssessmentResult](../resources/threatassessmentresult.md) object.

The following table shows the properties that are required when you create the [threatAssessmentResult](../resources/threatassessmentresult.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|resultType|threatAssessmentResultType|**TODO: Add Description**. Possible values are: `checkPolicy`, `rescan`, `unknownFutureValue`.|
|message|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [threatAssessmentResult](../resources/threatassessmentresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_threatassessmentresult_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests/{threatAssessmentRequestId}/results
Content-Type: application/json
Content-length: 115

{
  "@odata.type": "#microsoft.graph.threatAssessmentResult",
  "resultType": "String",
  "message": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatassessmentresult"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.threatAssessmentResult",
  "id": "b3bfe915-e915-b3bf-15e9-bfb315e9bfb3",
  "createdDateTime": "String (timestamp)",
  "resultType": "String",
  "message": "String"
}
```


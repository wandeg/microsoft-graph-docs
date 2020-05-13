---
title: "Create threatAssessmentRequests"
description: "Create a new threatAssessmentRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create threatAssessmentRequests

Namespace: microsoft.graph

Create a new threatAssessmentRequests object.

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
POST /informationProtection/threatAssessmentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.

The following table shows the properties that are required when you create the [threatAssessmentRequest](../resources/threatassessmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|contentType|threatAssessmentContentType|**TODO: Add Description**. Possible values are: `mail`, `url`, `file`.|
|expectedAssessment|threatExpectedAssessment|**TODO: Add Description**. Possible values are: `block`, `unblock`.|
|category|threatCategory|**TODO: Add Description**. Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|status|threatAssessmentStatus|**TODO: Add Description**. Possible values are: `pending`, `completed`.|
|requestSource|threatAssessmentRequestSource|**TODO: Add Description**. Possible values are: `undefined`, `user`, `administrator`.|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_threatassessmentrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/informationProtection/threatAssessmentRequests
Content-Type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.threatAssessmentRequest",
  "contentType": "String",
  "expectedAssessment": "String",
  "category": "String",
  "status": "String",
  "requestSource": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatassessmentrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.threatAssessmentRequest",
  "id": "5b8a753b-753b-5b8a-3b75-8a5b3b758a5b",
  "createdDateTime": "String (timestamp)",
  "contentType": "String",
  "expectedAssessment": "String",
  "category": "String",
  "status": "String",
  "requestSource": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


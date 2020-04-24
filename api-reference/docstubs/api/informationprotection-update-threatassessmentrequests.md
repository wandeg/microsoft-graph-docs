---
title: "Update threatAssessmentRequests"
description: "Update the properties of a threatAssessmentRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update threatAssessmentRequests

Namespace: microsoft.graph

Update the properties of a threatAssessmentRequests object.

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
PATCH /invitations/{invitationsId}/invitedUser/informationProtection/threatAssessmentRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

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
If successful, this method returns a `200 OK` response code and an updated [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_threatassessmentrequests"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/invitations/{invitationsId}/invitedUser/informationProtection/threatAssessmentRequests
Content-Type: application/json
Content-length: 574

{
  "@odata.type": "#microsoft.graph.threatAssessmentRequest",
  "contentType": "String",
  "expectedAssessment": "String",
  "category": "String",
  "status": "String",
  "requestSource": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
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
  "@odata.type": "#microsoft.graph.threatAssessmentRequest",
  "id": "f901db52-db52-f901-52db-01f952db01f9",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "contentType": "String",
  "expectedAssessment": "String",
  "category": "String",
  "status": "String",
  "requestSource": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet",
    "application": {
      "@odata.type": "microsoft.graph.identity",
      "id": "Id value",
      "displayName": "Display Name value"
    },
    "device": {
      "@odata.type": "microsoft.graph.identity"
    },
    "user": {
      "@odata.type": "microsoft.graph.identity"
    }
  }
}
```


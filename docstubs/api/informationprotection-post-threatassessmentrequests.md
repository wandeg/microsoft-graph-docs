---
title: "Add threatAssessmentRequests"
description: "Add threatAssessmentRequests by posting to the threatAssessmentRequests collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add threatAssessmentRequests

Namespace: microsoft.graph

Add threatAssessmentRequests by posting to the threatAssessmentRequests collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /informationProtection/threatAssessmentRequests/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [threatAssessmentRequest](../resources/threatassessmentrequest.md) object.

The following table shows the properties that are required when you create the [threatAssessmentRequest](../resources/threatassessmentrequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset||
|contentType|Enumeration| Possible values are: `mail`, `url`, `file`.|
|expectedAssessment|Enumeration| Possible values are: `block`, `unblock`.|
|category|Enumeration| Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|status|Enumeration| Possible values are: `pending`, `completed`.|
|requestSource|Enumeration| Possible values are: `undefined`, `user`, `administrator`.|
|createdBy|[identitySet](../resources/identityset.md)||



## Response
If successful, this method returns a `201 Created` response code and a [threatAssessmentRequest](../resources/threatassessmentrequest.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_threatassessmentrequest_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/informationProtection/threatAssessmentRequests
Content-type: application/json
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
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.threatassessmentrequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 682

{
  "@odata.type": "#microsoft.graph.threatAssessmentRequest",
  "id": "70162b74-2b74-7016-742b-1670742b1670",
  "createdDateTime": "2017-01-01T00:00:31.4223767+00:00",
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


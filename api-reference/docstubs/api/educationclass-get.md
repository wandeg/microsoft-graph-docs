---
title: "Get educationClass"
description: "Read the properties and relationships of an educationClass object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get educationClass

Namespace: microsoft.graph

Read the properties and relationships of an [educationClass](../resources/educationclass.md) object.

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
GET /education/classes/{educationClassId}
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
If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/classes/{educationClassId}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
{
  "value": {
    "@odata.type": "#microsoft.graph.educationClass",
    "id": "87421f6f-1f6f-8742-6f1f-42876f1f4287",
    "displayName": "Display Name value",
    "mailNickname": "Mail Nickname value",
    "description": "Description value",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet",
      "application": {
        "@odata.type": "microsoft.graph.identity",
        "id": "Id value"
      },
      "device": {
        "@odata.type": "microsoft.graph.identity"
      },
      "user": {
        "@odata.type": "microsoft.graph.identity"
      }
    },
    "classCode": "Class Code value",
    "externalName": "External Name value",
    "externalId": "External Id value",
    "externalSource": "String",
    "grade": "Grade value",
    "term": {
      "@odata.type": "microsoft.graph.educationTerm",
      "startDate": "Date",
      "endDate": "Date"
    },
    "course": {
      "@odata.type": "microsoft.graph.educationCourse",
      "subject": "Subject value",
      "courseNumber": "Course Number value"
    }
  }
}
```


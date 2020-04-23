---
title: "Update educationClass"
description: "Update the properties of an educationClass object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update educationClass

Namespace: microsoft.graph

Update the properties of an [educationClass](../resources/educationclass.md) object.

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
PATCH /education/classes/{educationClassId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [educationClass](../resources/educationclass.md) object.

The following table shows the properties that are required when you create the [educationClass](../resources/educationclass.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|mailNickname|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|classCode|String|**TODO: Add Description**|
|externalName|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|externalSource|educationExternalSource|**TODO: Add Description**. Possible values are: `sis`, `manual`, `unknownFutureValue`.|
|term|[educationTerm](../resources/educationterm.md)|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [educationClass](../resources/educationclass.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_educationclass"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}
Content-Type: application/json
Content-length: 769

{
  "@odata.type": "#microsoft.graph.educationClass",
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
  "term": {
    "@odata.type": "microsoft.graph.educationTerm",
    "startDate": "Date",
    "endDate": "Date"
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
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "24099195-9195-2409-9591-092495910924",
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
  "term": {
    "@odata.type": "microsoft.graph.educationTerm",
    "startDate": "Date",
    "endDate": "Date"
  }
}
```


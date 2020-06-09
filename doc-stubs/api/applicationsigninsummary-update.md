---
title: "Update applicationSignInSummary"
description: "Update the properties of an applicationSignInSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update applicationSignInSummary
Namespace: microsoft.graph

Update the properties of an [applicationSignInSummary](../resources/applicationsigninsummary.md) object.

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
PATCH /applicationSignInSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [applicationSignInSummary](../resources/applicationsigninsummary.md) object.

The following table shows the properties that are required when you create the [applicationSignInSummary](../resources/applicationsigninsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|appDisplayName|String|**TODO: Add Description**|
|successfulSignInCount|Int64|**TODO: Add Description**|
|failedSignInCount|Int64|**TODO: Add Description**|
|successPercentage|Double|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_applicationsigninsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applicationSignInSummary
Content-Type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.applicationSignInSummary",
  "appDisplayName": "String",
  "successfulSignInCount": "Integer",
  "failedSignInCount": "Integer",
  "successPercentage": "Double"
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
  "@odata.type": "#microsoft.graph.applicationSignInSummary",
  "id": "97916bba-6bba-9791-ba6b-9197ba6b9197",
  "appDisplayName": "String",
  "successfulSignInCount": "Integer",
  "failedSignInCount": "Integer",
  "successPercentage": "Double"
}
```


---
title: "Add groupPolicyOperations"
description: "Add groupPolicyOperations by posting to the groupPolicyOperations collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add groupPolicyOperations

Namespace: microsoft.graph

Add groupPolicyOperations by posting to the groupPolicyOperations collection.

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
POST ** Collection URI for microsoft.graph.groupPolicyOperation not found/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [groupPolicyOperation](../resources/grouppolicyoperation.md) object.

The following table shows the properties that are required when you create the [groupPolicyOperation](../resources/grouppolicyoperation.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|operationType|groupPolicyOperationType|The type of group policy operation. Possible values are: `none`, `upload`, `uploadNewVersion`, `addLanguageFiles`, `removeLanguageFiles`, `updateLanguageFiles`, `remove`.|
|operationStatus|groupPolicyOperationStatus|The group policy operation status. Possible values are: `unknown`, `inProgress`, `success`, `failed`.|
|statusDetails|String|The group policy operation status detail.|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|



## Response
If successful, this method returns a `204 No Content` response code and a [groupPolicyOperation](../resources/grouppolicyoperation.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_grouppolicyoperation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.groupPolicyOperation not found/$ref
Content-Type: application/json
Content-length: 168

{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "operationType": "String",
  "operationStatus": "String",
  "statusDetails": "Status Details value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.grouppolicyoperation"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.groupPolicyOperation",
  "id": "343412f5-12f5-3434-f512-3434f5123434",
  "operationType": "String",
  "operationStatus": "String",
  "statusDetails": "Status Details value",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00"
}
```


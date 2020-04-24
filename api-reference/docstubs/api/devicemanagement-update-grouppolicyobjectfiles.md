---
title: "Update groupPolicyObjectFiles"
description: "Update the properties of a groupPolicyObjectFiles object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update groupPolicyObjectFiles

Namespace: microsoft.graph

Update the properties of a groupPolicyObjectFiles object.

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
PATCH /deviceManagement/groupPolicyObjectFiles
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object.

The following table shows the properties that are required when you create the [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|groupPolicyObjectId|Guid|The Group Policy Object GUID from GPO Xml content|
|ouDistinguishedName|String|The distinguished name of the OU.|
|createdDateTime|DateTimeOffset|The date and time at which the GroupPolicy was first uploaded.|
|lastModifiedDateTime|DateTimeOffset|The date and time at which the GroupPolicyObjectFile was last modified.|
|content|String|The Group Policy Object file content.|



## Response
If successful, this method returns a `200 OK` response code and an updated [groupPolicyObjectFile](../resources/grouppolicyobjectfile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_grouppolicyobjectfiles"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyObjectFiles
Content-Type: application/json
Content-length: 217

{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "groupPolicyObjectId": "aa11b3d9-b3d9-aa11-d9b3-11aad9b311aa",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "content": "Content value"
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
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "65fa2f10-2f10-65fa-102f-fa65102ffa65",
  "groupPolicyObjectId": "aa11b3d9-b3d9-aa11-d9b3-11aad9b311aa",
  "ouDistinguishedName": "Ou Distinguished Name value",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "content": "Content value"
}
```


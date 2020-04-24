---
title: "Update items"
description: "Update the properties of an items object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update items

Namespace: microsoft.graph

Update the properties of an items object.

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
PATCH /deviceAppManagement/policySets/{policySetId}/items
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [policySetItem](../resources/policysetitem.md) object.

The following table shows the properties that are required when you create the [policySetItem](../resources/policysetitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|Creation time of the PolicySetItem.|
|lastModifiedDateTime|DateTimeOffset|Last modified time of the PolicySetItem.|
|payloadId|String|PayloadId of the PolicySetItem.|
|itemType|String|policySetType of the PolicySetItem.|
|displayName|String|DisplayName of the PolicySetItem.|
|status|policySetStatus|Status of the PolicySetItem. Possible values are: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|errorCode|Error code if any occured. Possible values are: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Tags of the guided deployment|



## Response
If successful, this method returns a `200 OK` response code and an updated [policySetItem](../resources/policysetitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_items"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items
Content-Type: application/json
Content-length: 285

{
  "@odata.type": "#microsoft.graph.policySetItem",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
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
  "@odata.type": "#microsoft.graph.policySetItem",
  "id": "864619c6-19c6-8646-c619-4686c6194686",
  "createdDateTime": "2016-12-31T23:57:10.8757278+03:00",
  "lastModifiedDateTime": "2016-12-31T23:59:40.8735716+03:00",
  "payloadId": "Payload Id value",
  "itemType": "Item Type value",
  "displayName": "Display Name value",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "Guided Deployment Tags value"
  ]
}
```


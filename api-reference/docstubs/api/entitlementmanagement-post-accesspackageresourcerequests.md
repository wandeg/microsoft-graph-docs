---
title: "Create accessPackageResourceRequests"
description: "Create a new accessPackageResourceRequests object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create accessPackageResourceRequests

Namespace: microsoft.graph

Create a new accessPackageResourceRequests object.

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
POST /identityGovernance/entitlementManagement/accessPackageResourceRequests
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object.

The following table shows the properties that are required when you create the [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|catalogId|String|**TODO: Add Description**|
|executeImmediately|Boolean|**TODO: Add Description**|
|isValidationOnly|Boolean|**TODO: Add Description**|
|requestType|String|**TODO: Add Description**|
|requestState|String|**TODO: Add Description**|
|requestStatus|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|justification|String|**TODO: Add Description**|



## Response
If successful, this method returns a `201 Created` response code and an [accessPackageResourceRequest](../resources/accesspackageresourcerequest.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_accesspackageresourcerequest_from_accesspackageresourcerequests"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageResourceRequests
Content-Type: application/json
Content-length: 396

{
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "catalogId": "Catalog Id value",
  "executeImmediately": true,
  "isValidationOnly": true,
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "justification": "Justification value"
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accesspackageresourcerequest"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceRequest",
  "id": "c4e1c7ee-c7ee-c4e1-eec7-e1c4eec7e1c4",
  "catalogId": "Catalog Id value",
  "executeImmediately": true,
  "isValidationOnly": true,
  "requestType": "Request Type value",
  "requestState": "Request State value",
  "requestStatus": "Request Status value",
  "expirationDateTime": "2016-12-31T23:56:37.756224+03:00",
  "justification": "Justification value"
}
```


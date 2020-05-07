---
title: "Update dataSharingConsents"
description: "Update the properties of a dataSharingConsents object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update dataSharingConsents

Namespace: microsoft.graph

Update the properties of a dataSharingConsents object.

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
PATCH /deviceManagement/dataSharingConsents
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [dataSharingConsent](../resources/datasharingconsent.md) object.

The following table shows the properties that are required when you create the [dataSharingConsent](../resources/datasharingconsent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|serviceDisplayName|String|**TODO: Add Description**|
|termsUrl|String|**TODO: Add Description**|
|granted|Boolean|**TODO: Add Description**|
|grantDateTime|DateTimeOffset|**TODO: Add Description**|
|grantedByUpn|String|**TODO: Add Description**|
|grantedByUserId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/datasharingconsent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_datasharingconsents"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents
Content-Type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": "Boolean",
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
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
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "168ffd95-fd95-168f-95fd-8f1695fd8f16",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": "Boolean",
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```


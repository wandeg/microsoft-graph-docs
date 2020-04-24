---
title: "Update applicationTemplate"
description: "Update the properties of an applicationTemplate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update applicationTemplate

Namespace: microsoft.graph

Update the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.

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
PATCH /applicationTemplates/{applicationTemplatesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [applicationTemplate](../resources/applicationtemplate.md) object.

The following table shows the properties that are required when you create the [applicationTemplate](../resources/applicationtemplate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|homePageUrl|String|**TODO: Add Description**|
|supportedSingleSignOnModes|String collection|**TODO: Add Description**|
|supportedProvisioningTypes|String collection|**TODO: Add Description**|
|logoUrl|String|**TODO: Add Description**|
|categories|String collection|**TODO: Add Description**|
|publisher|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|



## Response
If successful, this method returns a `200 OK` response code and an updated [applicationTemplate](../resources/applicationtemplate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_applicationtemplate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applicationTemplates/{applicationTemplatesId}
Content-Type: application/json
Content-length: 492

{
  "@odata.type": "#microsoft.graph.applicationTemplate",
  "displayName": "Display Name value",
  "homePageUrl": "https://example.com/homePageUrl/",
  "supportedSingleSignOnModes": [
    "Supported Single Sign On Modes value"
  ],
  "supportedProvisioningTypes": [
    "Supported Provisioning Types value"
  ],
  "logoUrl": "https://example.com/logoUrl/",
  "categories": [
    "Categories value"
  ],
  "publisher": "Publisher value",
  "description": "Description value"
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
  "@odata.type": "#microsoft.graph.applicationTemplate",
  "id": "6d063dee-3dee-6d06-ee3d-066dee3d066d",
  "displayName": "Display Name value",
  "homePageUrl": "https://example.com/homePageUrl/",
  "supportedSingleSignOnModes": [
    "Supported Single Sign On Modes value"
  ],
  "supportedProvisioningTypes": [
    "Supported Provisioning Types value"
  ],
  "logoUrl": "https://example.com/logoUrl/",
  "categories": [
    "Categories value"
  ],
  "publisher": "Publisher value",
  "description": "Description value"
}
```


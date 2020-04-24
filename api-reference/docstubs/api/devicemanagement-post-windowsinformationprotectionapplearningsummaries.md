---
title: "Create windowsInformationProtectionAppLearningSummaries"
description: "Create a new windowsInformationProtectionAppLearningSummaries object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create windowsInformationProtectionAppLearningSummaries

Namespace: microsoft.graph

Create a new windowsInformationProtectionAppLearningSummaries object.

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
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required|
|Content-Type|application/json. Required|

## Request body
In the request body, supply a JSON representation of the [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object.

The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|applicationName|String|Application Name|
|applicationType|applicationType|Application Type. Possible values are: `universal`, `desktop`.|
|deviceCount|Int32|Device Count|



## Response
If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLearningSummary](../resources/windowsinformationprotectionapplearningsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsinformationprotectionapplearningsummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-Type: application/json
Content-length: 190

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "String",
  "deviceCount": 11
}
```

### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsinformationprotectionapplearningsummary"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "568a16e9-16e9-568a-e916-8a56e9168a56",
  "applicationName": "Application Name value",
  "applicationType": "String",
  "deviceCount": 11
}
```


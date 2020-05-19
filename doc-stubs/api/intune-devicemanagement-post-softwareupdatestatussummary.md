---
title: "Add softwareUpdateStatusSummary"
description: "Add softwareUpdateStatusSummary by posting to the softwareUpdateStatusSummary collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add softwareUpdateStatusSummary

Namespace: microsoft.graph

Add softwareUpdateStatusSummary by posting to the softwareUpdateStatusSummary collection.

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
POST /deviceManagement/softwareUpdateStatusSummary/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [softwareUpdateStatusSummary](../resources/intune-softwareupdatestatussummary.md) object.

The following table shows the properties that are required when you create the [softwareUpdateStatusSummary](../resources/intune-softwareupdatestatussummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|compliantDeviceCount|Int32|**TODO: Add Description**|
|nonCompliantDeviceCount|Int32|**TODO: Add Description**|
|remediatedDeviceCount|Int32|**TODO: Add Description**|
|errorDeviceCount|Int32|**TODO: Add Description**|
|unknownDeviceCount|Int32|**TODO: Add Description**|
|conflictDeviceCount|Int32|**TODO: Add Description**|
|notApplicableDeviceCount|Int32|**TODO: Add Description**|
|compliantUserCount|Int32|**TODO: Add Description**|
|nonCompliantUserCount|Int32|**TODO: Add Description**|
|remediatedUserCount|Int32|**TODO: Add Description**|
|errorUserCount|Int32|**TODO: Add Description**|
|unknownUserCount|Int32|**TODO: Add Description**|
|conflictUserCount|Int32|**TODO: Add Description**|
|notApplicableUserCount|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [softwareUpdateStatusSummary](../resources/intune-softwareupdatestatussummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_softwareupdatestatussummary_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary/$ref
Content-Type: application/json
Content-length: 617

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "displayName": "String",
  "compliantDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "unknownDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantUserCount": "Integer",
  "nonCompliantUserCount": "Integer",
  "remediatedUserCount": "Integer",
  "errorUserCount": "Integer",
  "unknownUserCount": "Integer",
  "conflictUserCount": "Integer",
  "notApplicableUserCount": "Integer"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.softwareupdatestatussummary"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "b4c9137c-137c-b4c9-7c13-c9b47c13c9b4",
  "displayName": "String",
  "compliantDeviceCount": "Integer",
  "nonCompliantDeviceCount": "Integer",
  "remediatedDeviceCount": "Integer",
  "errorDeviceCount": "Integer",
  "unknownDeviceCount": "Integer",
  "conflictDeviceCount": "Integer",
  "notApplicableDeviceCount": "Integer",
  "compliantUserCount": "Integer",
  "nonCompliantUserCount": "Integer",
  "remediatedUserCount": "Integer",
  "errorUserCount": "Integer",
  "unknownUserCount": "Integer",
  "conflictUserCount": "Integer",
  "notApplicableUserCount": "Integer"
}
```


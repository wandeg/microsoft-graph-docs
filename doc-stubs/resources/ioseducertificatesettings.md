---
title: "iosEduCertificateSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosEduCertificateSettings resource type


Namespace: microsoft.graph

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|certFileName|String|**TODO: Add Description**|
|certificateTemplateName|String|**TODO: Add Description**|
|certificateValidityPeriodScale|certificateValidityPeriodScale|**TODO: Add Description**. Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32|**TODO: Add Description**|
|certificationAuthority|String|**TODO: Add Description**|
|certificationAuthorityName|String|**TODO: Add Description**|
|renewalThresholdPercentage|Int32|**TODO: Add Description**|
|trustedRootCertificate|Binary|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "Binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": "Integer",
  "certificateValidityPeriodValue": "Integer",
  "certificateValidityPeriodScale": "String"
}
```


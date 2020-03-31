---
title: "iosEduCertificateSettings resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# iosEduCertificateSettings resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|certFileName|String||
|certificateTemplateName|String||
|certificateValidityPeriodScale|Enumeration| Possible values are: `days`, `months`, `years`.|
|certificateValidityPeriodValue|Int32||
|certificationAuthority|String||
|certificationAuthorityName|String||
|renewalThresholdPercentage|Int32||
|trustedRootCertificate|Binary||

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosEduCertificateSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduCertificateSettings",
  "trustedRootCertificate": "binary",
  "certFileName": "String",
  "certificationAuthority": "String",
  "certificationAuthorityName": "String",
  "certificateTemplateName": "String",
  "renewalThresholdPercentage": 1024,
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```


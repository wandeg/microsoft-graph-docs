---
title: "windowsDeviceHealthState enum type"
description: "Computer endpoint protection state"
localization_priority: Normal
author: "$(metadata.owner)"
ms.prod: ""
doc_type: enumPageType
---

# windowsDeviceHealthState enum type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Computer endpoint protection state

## Members

| Member             | Value | Description                                 |
| :----------------- | ----: | :------------------------------------------ |
| clean              | 0     | Computer is clean and no action is required |
| fullScanPending    | 1     | Computer is in pending full scan state      |
| rebootPending      | 2     | Computer is in pending reboot state         |
| manualStepsPending | 4     | Computer is in pending manual steps state   |
| offlineScanPending | 8     | Computer is in pending offline scan state   |
| critical           | 16    | Computer is in critical failure state       |
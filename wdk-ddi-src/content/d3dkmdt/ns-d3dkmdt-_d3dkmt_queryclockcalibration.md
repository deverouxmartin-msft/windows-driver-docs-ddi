---
UID: NS:d3dkmdt._D3DKMT_QUERYCLOCKCALIBRATION
title: _D3DKMT_QUERYCLOCKCALIBRATION
author: windows-driver-content
description: Arguments used to query clock calibration information.
ms.assetid: b58027b5-e51b-4eb2-b8f0-0400be664995
ms.author: windowsdriverdev
ms.date: 
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: _D3DKMT_QUERYCLOCKCALIBRATION, D3DKMT_QUERYCLOCKCALIBRATION, 
req.header: d3dkmdt.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.ddi-compliance:
req.unicode-ansi:
req.max-support:
req.typenames: D3DKMT_QUERYCLOCKCALIBRATION
topic_type: 
-	apiref
api_type: 
-	HeaderDef
api_location: 
-	d3dkmdt.h
api_name: 
-	_D3DKMT_QUERYCLOCKCALIBRATION
product:
-	Windows
targetos: Windows
---

# _D3DKMT_QUERYCLOCKCALIBRATION structure

## -description

Arguments used to query clock calibration information.

## -struct-fields

### -field hAdapter

[in] The adapter to query clock information for.

### -field NodeOrdinal

[in] Node ordinal of the requested engine.

### -field PhysicalAdapterIndex

[in] The physical adapter index, in an LDA chain.

### -field ClockData
 
[out] Output frequency, GPU clock, and CPU clock on the specified engine.

## -remarks

## -see-also
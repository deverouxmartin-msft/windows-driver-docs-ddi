---
UID: NS:d3dkmddi._DXGKARG_RESUMEHWENGINE
title: _DXGKARG_RESUMEHWENGINE
author: windows-driver-content
description: Arguments used to resume the hardware engine.
ms.assetid: 745bf4ce-87ca-4471-b162-5687380ae09c
ms.author: windowsdriverdev
ms.date:
ms.topic: struct
ms.prod: windows-hardware
ms.technology: windows-devices
ms.keywords: _DXGKARG_RESUMEHWENGINE, DXGKARG_RESUMEHWENGINE, *INOUT_PDXGKARG_RESUMEHWENGINE
req.header: d3dkmddi.h
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
req.typenames: DXGKARG_RESUMEHWENGINE
topic_type:
-	apiref
api_type:
-	HeaderDef
api_location:
-	d3dkmddi.h
api_name:
-	_DXGKARG_RESUMEHWENGINE
product:
-	Windows
targetos: Windows
tech.root: display
---

# _DXGKARG_RESUMEHWENGINE structure

## -description

Contains arguments used to resume the hardware engine.

## -struct-fields

### -field NodeOrdinal

GPU node ordinal for the GPU engine that is being requested to resume.

### -field EngineOrdinal

GPU engine ordinal being requested to resume.


## -see-also

[DXGKDDI_RESUMEHWENGINE](nc-d3dkmddi-dxgkddi_resumehwengine.md)
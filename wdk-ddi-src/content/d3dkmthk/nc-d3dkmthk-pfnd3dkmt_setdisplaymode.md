---
UID: NC:d3dkmthk.PFND3DKMT_SETDISPLAYMODE
title: PFND3DKMT_SETDISPLAYMODE
author: windows-driver-content
description: The PFND3DKMT_SETDISPLAYMODE callback function sets the allocation that is used to scan out to the display.
ms.assetid: 354a3cdc-f353-4c11-bd41-391ac936886a
ms.author: windowsdriverdev
ms.date: 
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: d3dkmthk.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
req.irql: 
req.ddi-compliance:
req.unicode-ansi:
req.idl:
req.max-support:
req.namespace:
req.assembly:
req.type-library: 
topic_type: 
-	apiref
api_type: 
-	UserDefined
api_location: 
-	d3dkmthk.h
api_name: 
-	PFND3DKMT_SETDISPLAYMODE
product:
-	Windows
targetos: Windows
---

# PFND3DKMT_SETDISPLAYMODE callback function

## -description

The PFND3DKMT_SETDISPLAYMODE callback function sets the allocation that is used to scan out to the display.

## -prototype

```
//Declaration

PFND3DKMT_SETDISPLAYMODE Pfnd3dkmtSetdisplaymode; 

// Definition

NTSTATUS Pfnd3dkmtSetdisplaymode 
(
	const D3DKMT_SETDISPLAYMODE *
)
{...}

```

## -parameters

### -param * 

Pointer to a [D3DKMT_SETDISPLAYMODE](ns-d3dkmthk-_d3dkmt_setdisplaymode.md) structure.

## -returns

Returns NTSTATUS.


## -remarks




## -see-also
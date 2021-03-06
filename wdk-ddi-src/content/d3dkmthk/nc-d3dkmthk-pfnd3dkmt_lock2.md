---
UID: NC:d3dkmthk.PFND3DKMT_LOCK2
title: PFND3DKMT_LOCK2
author: windows-driver-content
description: Pfnd3dkmtLock2 locks an entire allocation or specific pages within an allocation.
ms.assetid: d06f98d8-dec7-4330-b3de-845205cf1ca3
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
-	PFND3DKMT_LOCK2
product:
-	Windows
targetos: Windows
---

# PFND3DKMT_LOCK2 callback function

## -description

Pfnd3dkmtLock2 locks an entire allocation or specific pages within an allocation.

## -prototype

```
//Declaration

PFND3DKMT_LOCK2 Pfnd3dkmtLock2; 

// Definition

NTSTATUS Pfnd3dkmtLock2 
(
	D3DKMT_LOCK2 *
)
{...}

```

## -parameters

### -param * 

Pointer to a [D3DKMT_LOCK2](ns-d3dkmthk-_d3dkmt_lock2.md) structure.

## -returns

Returns NTSTATUS.


## -remarks




## -see-also
---
UID: NC:d3d10umddi.PFND3DWDDM2_2DDI_SET_SHADERCACHE_SESSION
title: PFND3DWDDM2_2DDI_SET_SHADERCACHE_SESSION
author: windows-driver-content
description: The pfnSetShaderCacheSession callback function sets a shader cache session.
old-location: display\pfnd3dwddm2_2ddi_set_shadercache_session.htm
ms.assetid: 18BA159D-5E78-41AC-8CB8-97AEC2AE9592
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: PFND3DWDDM2_2DDI_SET_SHADERCACHE_SESSION, PFND3DWDDM2_2DDI_SET_SHADERCACHE_SESSION callback, d3d10umddi/pfnSetShaderCacheSession, display.pfnd3dwddm2_2ddi_set_shadercache_session, pfnSetShaderCacheSession, pfnSetShaderCacheSession callback function [Display Devices]
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: callback
req.header: d3d10umddi.h
req.include-header: D3d12umddi.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	UserDefined
api_location:
-	d3d10umddi.h
api_name:
-	pfnSetShaderCacheSession
product:
- Windows
targetos: Windows
tech.root: display
req.typenames: 
---

# PFND3DWDDM2_2DDI_SET_SHADERCACHE_SESSION callback function


## -description


The <i>pfnSetShaderCacheSession</i> callback function sets a shader cache session.


## -parameters




### -param Arg1

*hDevice*

A handle to the display device (graphics context).

### -param Arg2

*hCacheSession*

The handle of a cache session.




## -returns



This callback function does not return a value.




## -remarks



Access this callback function by using the <a href="https://msdn.microsoft.com/4E082193-70BA-4F36-9001-2A12014F3AC3">D3DWDDM2_2DDI_DEVICEFUNCS</a> structure. 




## -see-also




<a href="https://msdn.microsoft.com/4E082193-70BA-4F36-9001-2A12014F3AC3">D3DWDDM2_2DDI_DEVICEFUNCS</a>
 

 


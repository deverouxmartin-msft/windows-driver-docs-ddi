---
UID: NF:storport.StorPortReadRegisterUlong64
title: StorPortReadRegisterUlong64 macro
author: windows-driver-content
description: The StorPortReadRegisterUlong64 routine reads a 64-bit value from a specified 64-bit register address.
old-location: storage\storportreadregisterulong64.htm
tech.root: storage
ms.assetid: 73A9E645-0B71-429F-9033-032BB83E60E4
ms.author: windowsdriverdev
ms.date: 3/29/2018
ms.keywords: StorPortReadRegisterUlong64, StorPortReadRegisterUlong64 routine [Storage Devices], storage.storportreadregisterulong64, storport/StorPortReadRegisterUlong64
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: macro
req.header: storport.h
req.include-header: Storport.h
req.target-type: Universal
req.target-min-winverclnt: Available starting with Windows 8.
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
-	HeaderDef
api_location:
-	storport.h
api_name:
-	StorPortReadRegisterUlong64
product:
- Windows
targetos: Windows
req.typenames: 
---

# StorPortReadRegisterUlong64 macro


## -description


The <b>StorPortReadRegisterUlong64</b> routine reads a 64-bit value from a specified 64-bit register address.


## -parameters




### -param h [in]

A pointer to the hardware device extension.


### -param r [in]

A pointer to the register where the data is to be read. 

## -remarks



The <b>StorPortReadRegisterUlong64</b> routine is only available on the 64-bit version of Windows.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/hh967743">StorPortWriteRegisterUlong64</a>
 

 


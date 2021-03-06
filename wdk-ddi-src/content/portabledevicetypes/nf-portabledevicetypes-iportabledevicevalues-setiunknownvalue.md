---
UID: NF:portabledevicetypes.IPortableDeviceValues.SetIUnknownValue
title: IPortableDeviceValues::SetIUnknownValue
author: windows-driver-content
description: Adds a new IUnknown value (type VT_UNKNOWN) or overwrites an existing one.
old-location: wpddk\iportabledevicevalues_setiunknownvalue.htm
tech.root: wpd_dk
ms.assetid: 776d4097-a582-4708-8965-0dc956d73e0d
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: IPortableDeviceValues interface,SetIUnknownValue method, IPortableDeviceValues.SetIUnknownValue, IPortableDeviceValues::SetIUnknownValue, IPortableDeviceValuesSetIUnknownValue, SetIUnknownValue, SetIUnknownValue method, SetIUnknownValue method,IPortableDeviceValues interface, portabledevicetypes/IPortableDeviceValues::SetIUnknownValue, wpddk.iportabledevicevalues_setiunknownvalue
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: portabledevicetypes.h
req.include-header: 
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
-	COM
api_location:
-	PortableDeviceTypes.h
api_name:
-	IPortableDeviceValues.SetIUnknownValue
product:
-	Windows
targetos: Windows
req.typenames: 
---

# IPortableDeviceValues::SetIUnknownValue


## -description



Adds a new <b>IUnknown</b> value (type VT_UNKNOWN) or overwrites an existing one.




## -parameters




### -param key [in]

A <b>REFPROPERTYKEY</b> that specifies the item to create or overwrite.


### -param pValue [in]

A pointer to an <b>IUnknown</b> interface that specifies the new value. The SDK copies a reference to the submitted interface and calls <b>AddRef</b> on it.


## -returns



The method returns an <b>HRESULT</b>. Possible values include, but are not limited to, those in the following table.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method succeeded.

</td>
</tr>
</table>
 




## -remarks



If an existing value has the same key that is specified by the <i>key</i> parameter, it overwrites the existing value without any warning. The existing key memory is released appropriately.




## -see-also




<a href="https://msdn.microsoft.com/4a97301a-12cc-442f-a080-446ec9e1e245">IPortableDeviceValues Interface</a>



<a href="https://msdn.microsoft.com/ae66a86c-bf63-4bc7-87db-9d464004519a">IPortableDeviceValues::GetIUnknownValue</a>
 

 


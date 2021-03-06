---
UID: NS:portcls.__unnamed_struct_0c93_8
title: "*PPCNODE_DESCRIPTOR"
author: windows-driver-content
description: The PCNODE_DESCRIPTOR structure describes a node in the filter that a topology miniport driver implements.
old-location: audio\pcnode_descriptor.htm
tech.root: audio
ms.assetid: e83051ca-07fa-439d-8b0f-cbe6d84679a7
ms.author: windowsdriverdev
ms.date: 12/14/2017
ms.keywords: portcls/PPCNODE_DESCRIPTOR, PCNODE_DESCRIPTOR structure [Audio Devices], audpc-struct_275973f3-8db9-4b2c-ad30-e375b5e69656.xml, *PPCNODE_DESCRIPTOR, PPCNODE_DESCRIPTOR, audio.pcnode_descriptor, portcls/PCNODE_DESCRIPTOR, PPCNODE_DESCRIPTOR structure pointer [Audio Devices], PCNODE_DESCRIPTOR
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: portcls.h
req.include-header: Portcls.h
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
req.irql: PASSIVE_LEVEL
topictype:
-	APIRef
-	kbSyntax
apitype:
-	HeaderDef
apilocation:
-	portcls.h
apiname:
-	PCNODE_DESCRIPTOR
product:
- Windows
targetos: Windows
req.typenames: "*PPCNODE_DESCRIPTOR, PCNODE_DESCRIPTOR"
---

# *PPCNODE_DESCRIPTOR structure


## -description


The <b>PCNODE_DESCRIPTOR</b> structure describes a node in the filter that a topology miniport driver implements.


## -syntax


````
typedef struct {
  ULONG                    Flags;
  const PCAUTOMATION_TABLE *AutomationTable;
  const GUID               *Type;
  const GUID               *Name;
} PCNODE_DESCRIPTOR, *PPCNODE_DESCRIPTOR;
````


## -struct-fields




### -field portcls.Flags




### -field portcls.AutomationTable




### -field portcls.Type




### -field portcls.Name





#### - Flags

Set to zero. No flag bits are currently defined.


#### - AutomationTable

Pointer to the automation table, which is a structure of type <a href="..\portcls\ns-portcls-__unnamed_struct_0c93_6.md">PCAUTOMATION_TABLE</a>. This member can be set to <b>NULL</b> to indicate no automation support. The automation table specifies the handlers for the properties and events belonging to the node instance.


#### - Type

Specifies the node type. This member is a pointer to a GUID that uniquely identifies the node type. See the list of node-type GUIDs in <a href="https://msdn.microsoft.com/library/windows/hardware/ff536219">Audio Topology Nodes</a>.


#### - Name

Pointer to a GUID that represents the name of this topology node. This GUID is specified in a <a href="https://msdn.microsoft.com/library/windows/hardware/ff565809">KSPROPERTY_TOPOLOGY_NAME</a>get-property request to obtain the corresponding name string for the node. This pointer can be set to <b>NULL</b> to indicate that the GUID in the <b>Type</b> member should be used to determine the node name.


## -remarks


If a filter contains only a single node of the type specified by the <b>Type</b> member, then the <b>Name</b> member can be specified as <b>NULL</b> because the <b>Type</b> value is sufficient to uniquely identify the node within the filter. If the filter contains two or more nodes of the same type, the <b>Name</b> members for those nodes must be non-<b>NULL</b>.

For example, if a filter contains a single SUM node, the <b>Type</b> member for that node points to GUID value <a href="https://msdn.microsoft.com/library/windows/hardware/ff537196">KSNODETYPE_SUM</a>, and the <b>Name</b> member is set to <b>NULL</b>. When queried for the name of that node, the <a href="https://msdn.microsoft.com/library/windows/hardware/ff565809">KSPROPERTY_TOPOLOGY_NAME</a> property, after determining that the node's <b>Name</b> value is <b>NULL</b>, retrieves the name string from the registry entry for the KSNODETYPE_SUM GUID. However, the same filter might contain several volume nodes, in which case the <b>Type</b> values for these nodes all point to the same GUID value, <a href="https://msdn.microsoft.com/library/windows/hardware/ff537208">KSNODETYPE_VOLUME</a>, and the <b>Name</b> value must uniquely identify each of the volume nodes. The <b>Name</b> value for the wave-input volume control node, for example, should point to GUID value KSAUDFNAME_WAVE_IN_VOLUME (defined in ksmedia.h). The registry entry for this GUID contains the name string that the KSPROPERTY_TOPOLOGY_NAME property retrieves for the node.

The <a href="..\portcls\ns-portcls-__unnamed_struct_0c93_9.md">PCFILTER_DESCRIPTOR</a> structure contains a pointer to an array of <b>PCNODE_DESCRIPTOR</b> structures.

For a simple code example that shows how the <b>PCNODE_DESCRIPTOR</b> structure is used, see <a href="https://msdn.microsoft.com/bf791f40-b2fb-48fe-8350-3b926db4ead7">Exposing Filter Topology</a>.



## -see-also

<a href="..\portcls\ns-portcls-__unnamed_struct_0c93_6.md">PCAUTOMATION_TABLE</a>

<a href="..\portcls\ns-portcls-__unnamed_struct_0c93_9.md">PCFILTER_DESCRIPTOR</a>

<a href="https://msdn.microsoft.com/library/windows/hardware/ff565809">KSPROPERTY_TOPOLOGY_NAME</a>

 

 



---
UID: NF:d3d10.ID3D10Device.CreateBuffer
title: ID3D10Device::CreateBuffer
author: windows-sdk-content
description: Create a buffer (vertex buffer, index buffer, or shader-constant buffer).
old-location: direct3d10\id3d10device_createbuffer.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10device_createbuffer.htm
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: CreateBuffer, CreateBuffer method [Direct3D 10], CreateBuffer method [Direct3D 10],ID3D10Device interface, ID3D10Device interface [Direct3D 10],CreateBuffer method, ID3D10Device.CreateBuffer, ID3D10Device::CreateBuffer, d3d10/ID3D10Device::CreateBuffer, direct3d10.id3d10device_createbuffer, f67833a5-95f8-0430-5015-e074533c6dd1
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d10.h
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
req.lib: D3D10.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D10.lib
 - D3D10.dll
api_name:
 - ID3D10Device.CreateBuffer
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- COM
: 
- d3d10.h
: 
- ID3D10Device.CreateBuffer
: 
---

# ID3D10Device::CreateBuffer


## -description


Create a <a href="https://msdn.microsoft.com/c5238a2f-d69d-4ce5-a5aa-66a6c18d5f69">buffer</a> (vertex buffer, index buffer, or shader-constant buffer).


## -parameters




### -param pDesc [in]

Type: <b>const <a href="https://msdn.microsoft.com/3f98c741-ff4c-4080-bd57-ef35cd6622d6">D3D10_BUFFER_DESC</a>*</b>

Pointer to a buffer description (see <a href="https://msdn.microsoft.com/3f98c741-ff4c-4080-bd57-ef35cd6622d6">D3D10_BUFFER_DESC</a>).


### -param pInitialData [in]

Type: <b>const <a href="https://msdn.microsoft.com/083d9027-5c4d-47f4-9d42-b1016628b210">D3D10_SUBRESOURCE_DATA</a>*</b>

Pointer to the initialization data (see <a href="https://msdn.microsoft.com/083d9027-5c4d-47f4-9d42-b1016628b210">D3D10_SUBRESOURCE_DATA</a>); use <b>NULL</b> to allocate space only.


### -param ppBuffer [out]

Type: <b><a href="https://msdn.microsoft.com/a81e0dfc-9be4-4ba6-a388-9c9bb97a0fa9">ID3D10Buffer</a>**</b>

Address of a pointer to the buffer created (see <a href="https://msdn.microsoft.com/a81e0dfc-9be4-4ba6-a388-9c9bb97a0fa9">ID3D10Buffer Interface</a>). Set this parameter to <b>NULL</b> to validate the other input parameters (S_FALSE indicates a pass).


## -returns



Type: <b><a href="455d07e9-52c3-4efb-a9dc-2955cbfd38cc">HRESULT</a></b>

This method returns one of the following <a href="https://msdn.microsoft.com/7b67d428-d000-4c3e-adc1-b5fc67a15a6a">Direct3D 10 Return Codes</a>.




## -remarks



For example code, see:

<ul>
<li>
<a href="https://msdn.microsoft.com/9787b153-9301-4a0f-bd6f-21cc6f7fc650">Create a Vertex Buffer</a>
</li>
<li>
<a href="https://msdn.microsoft.com/9787b153-9301-4a0f-bd6f-21cc6f7fc650">Create an Index Buffer</a>
</li>
</ul>



## -see-also




<a href="https://msdn.microsoft.com/63c7fca3-5575-41a7-9bdf-2582e6b9c182">ID3D10Device Interface</a>
 

 


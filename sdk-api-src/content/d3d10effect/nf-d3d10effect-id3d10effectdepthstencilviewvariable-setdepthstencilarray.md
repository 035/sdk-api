---
UID: NF:d3d10effect.ID3D10EffectDepthStencilViewVariable.SetDepthStencilArray
title: ID3D10EffectDepthStencilViewVariable::SetDepthStencilArray
author: windows-sdk-content
description: Set an array of depth-stencil-view resources.
old-location: direct3d10\id3d10effectdepthstencilviewvariable_setdepthstencilarray.htm
tech.root: direct3d10
ms.assetid: VS|directx_sdk|~\id3d10effectdepthstencilviewvariable_setdepthstencilarray.htm
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: 19d677a4-86e6-d451-5d65-7ab228f247d5, ID3D10EffectDepthStencilViewVariable interface [Direct3D 10],SetDepthStencilArray method, ID3D10EffectDepthStencilViewVariable.SetDepthStencilArray, ID3D10EffectDepthStencilViewVariable::SetDepthStencilArray, SetDepthStencilArray, SetDepthStencilArray method [Direct3D 10], SetDepthStencilArray method [Direct3D 10],ID3D10EffectDepthStencilViewVariable interface, d3d10effect/ID3D10EffectDepthStencilViewVariable::SetDepthStencilArray, direct3d10.id3d10effectdepthstencilviewvariable_setdepthstencilarray
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d10effect.h
req.include-header: D3d10
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
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - d3d10effect.h
api_name:
 - ID3D10EffectDepthStencilViewVariable.SetDepthStencilArray
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
---

# ID3D10EffectDepthStencilViewVariable::SetDepthStencilArray


## -description


Set an array of depth-stencil-view resources.


## -parameters




### -param ppResources [out]

Type: <b><a href="https://msdn.microsoft.com/b88f3b61-4549-4ef7-9dda-0c2ed247d2f1">ID3D10DepthStencilView</a>**</b>

A pointer to an array of depth-stencil-view interfaces. See <a href="https://msdn.microsoft.com/b88f3b61-4549-4ef7-9dda-0c2ed247d2f1">ID3D10DepthStencilView Interface</a>.


### -param Offset [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The zero-based array index to set the first interface.


### -param Count [in]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">UINT</a></b>

The number of elements in the array.


## -returns



Type: <b><a href="455d07e9-52c3-4efb-a9dc-2955cbfd38cc">HRESULT</a></b>

Returns one of the following <a href="https://msdn.microsoft.com/7b67d428-d000-4c3e-adc1-b5fc67a15a6a">Direct3D 10 Return Codes</a>.




## -see-also




<a href="https://msdn.microsoft.com/4d945731-aab6-40ac-8c07-d9a480c13a9c">ID3D10EffectDepthStencilViewVariable Interface</a>
 

 


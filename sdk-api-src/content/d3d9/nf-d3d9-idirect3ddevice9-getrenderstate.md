---
UID: NF:d3d9.IDirect3DDevice9.GetRenderState
title: IDirect3DDevice9::GetRenderState
author: windows-sdk-content
description: Retrieves a render-state value for a device.
old-location: direct3d9\idirect3ddevice9__getrenderstate.htm
tech.root: direct3d9
ms.assetid: VS|directx_sdk|~\idirect3ddevice9__getrenderstate.htm
ms.author: windowssdkdev
ms.date: 11/02/2018
ms.keywords: 2d20be3d-5ba4-bf91-6270-0a3b1c346d9d, GetRenderState, GetRenderState method [Direct3D 9], GetRenderState method [Direct3D 9],IDirect3DDevice9 interface, IDirect3DDevice9 interface [Direct3D 9],GetRenderState method, IDirect3DDevice9.GetRenderState, IDirect3DDevice9::GetRenderState, d3d9helper/IDirect3DDevice9::GetRenderState, direct3d9.idirect3ddevice9__getrenderstate
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: d3d9.h
req.include-header: D3D9.h
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
req.lib: D3D9.lib
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - D3D9.lib
 - D3D9.dll
api_name:
 - IDirect3DDevice9.GetRenderState
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- COM
: 
- d3d9.h
: 
- IDirect3DDevice9.GetRenderState
: 
---

# IDirect3DDevice9::GetRenderState


## -description


Retrieves a render-state value for a device.


## -parameters




### -param State [in]

Type: <b><a href="https://msdn.microsoft.com/2fd56388-f3bd-409f-876c-ae893840b623">D3DRENDERSTATETYPE</a></b>

Device state variable that is being queried. This parameter can be any member of the <a href="https://msdn.microsoft.com/2fd56388-f3bd-409f-876c-ae893840b623">D3DRENDERSTATETYPE</a> enumerated type. 


### -param pValue [out, retval]

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">DWORD</a>*</b>

Pointer to a variable that receives the value of the queried render state variable when the method returns. 


## -returns



Type: <b><a href="455d07e9-52c3-4efb-a9dc-2955cbfd38cc">HRESULT</a></b>

If the method succeeds, the return value is D3D_OK. D3DERR_INVALIDCALL if one of the arguments is invalid.




## -remarks



This method will not return device state for a device that is created using D3DCREATE_PUREDEVICE. If you want to use this method, you must create your device with any of the other values in <a href="https://msdn.microsoft.com/91387a2d-3927-4285-a09b-9ce247e6bfdd">D3DCREATE</a>."
    





## -see-also




<a href="https://msdn.microsoft.com/cf951e8e-7adb-417a-bda0-9b3cde4912a7">IDirect3DDevice9</a>



<a href="https://msdn.microsoft.com/65738aae-aa90-48c5-8c9c-1927d1c92c54">IDirect3DDevice9::SetRenderState</a>
 

 


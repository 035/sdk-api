---
UID: NF:mileffects.IMILBitmapEffectGroupImpl.GetChildren
title: IMILBitmapEffectGroupImpl::GetChildren
author: windows-sdk-content
description: Gets the children of the effect group.
old-location: wibe\_wibe_imilbitmapeffectgroupimpl_getchildren.htm
tech.root: wibe
ms.assetid: VS|wibe|~\wibelh\reference\ifaces\imilbitmapeffectgroupimpl\getchildren.htm
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: GetChildren, GetChildren method [WPF Bitmap Effects], GetChildren method [WPF Bitmap Effects],IMILBitmapEffectGroupImpl interface, IMILBitmapEffectGroupImpl interface [WPF Bitmap Effects],GetChildren method, IMILBitmapEffectGroupImpl.GetChildren, IMILBitmapEffectGroupImpl::GetChildren, _wibe_imilbitmapeffectgroupimpl_getchildren, mileffects/IMILBitmapEffectGroupImpl::GetChildren, wibe._wibe_imilbitmapeffectgroupimpl_getchildren
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: mileffects.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows XP with SP2, Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2008 [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Mileffects.idl
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
 - Mileffects.h
api_name:
 - IMILBitmapEffectGroupImpl.GetChildren
product: Windows
targetos: Windows
req.typenames: 
req.redist: Microsoft .Net 3.0
---

# IMILBitmapEffectGroupImpl::GetChildren


## -description


Gets the children of the effect group.


## -parameters




### -param pChildren [out, retval]

Type: <b><a href="https://msdn.microsoft.com/96ab3239-b739-4f05-a9ac-3da7ae059fcc">IMILBitmapEffects</a>**</b>

A pointer that receives a pointer to the <a href="https://msdn.microsoft.com/96ab3239-b739-4f05-a9ac-3da7ae059fcc">IMILBitmapEffects</a> group.


## -returns



Type: <b>HRESULT</b>

If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




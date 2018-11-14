---
UID: NF:gdipluspen.Pen.GetDashOffset
title: Pen::GetDashOffset
author: windows-sdk-content
description: The Pen::GetDashOffset method gets the distance from the start of the line to the start of the first space in a dashed line.
old-location: gdiplus\_gdiplus_CLASS_Pen_GetDashOffset_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\penclass\penmethods\getdashoffset.htm
ms.author: windowssdkdev
ms.date: 11/09/2018
ms.keywords: GetDashOffset, GetDashOffset method [GDI+], GetDashOffset method [GDI+],Pen class, Pen class [GDI+],GetDashOffset method, Pen.GetDashOffset, Pen::GetDashOffset, _gdiplus_CLASS_Pen_GetDashOffset_, gdiplus._gdiplus_CLASS_Pen_GetDashOffset_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdipluspen.h
req.include-header: Gdiplus.h
req.target-type: Windows
req.target-min-winverclnt: Windows XP, Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Gdiplus.lib
req.dll: Gdiplus.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Gdiplus.dll
api_name:
 - Pen.GetDashOffset
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- COM
: 
- gdipluspen.h
: 
- Pen.GetDashOffset
: 
req.product: GDI+ 1.0
---

# Pen::GetDashOffset


## -description


The <b>Pen::GetDashOffset</b> method gets the distance from the start of the line to the start of the first space in a dashed line.


## -parameters






## -returns



Type: <strong>Type: <b>REAL</b>
</strong>

This method returns a real number that indicates the distance from the start of the line to the start of the dashes.




## -remarks



A positive return value shifts the first dash forward along the path, and a negative return value shifts the start of the path forward along the first dash. 


#### Examples



The following example assumes that 
						<i>dashPen</i> has been defined with a certain dash style and gets the dash offset value.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>REAL dashOffset = dashPen.GetDashOffset();</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/0e75de3b-1006-4c8f-875c-eeb0782f24b0">Drawing a Custom Dashed Line</a>



<a href="https://msdn.microsoft.com/b48affa5-d953-478c-b651-0534db4d2b78">Pen</a>



<a href="https://msdn.microsoft.com/7d60736d-76e0-47d8-a138-7d9665741f10">Pen::SetDashOffset</a>



<a href="https://msdn.microsoft.com/d91562ab-41e6-4bca-a320-74f490a4f88f">Pens, Lines, and Rectangles</a>
 

 


---
UID: NF:gdipluspath.PathGradientBrush.SetCenterColor
title: PathGradientBrush::SetCenterColor
author: windows-sdk-content
description: The PathGradientBrush::SetCenterColor method sets the center color of this path gradient brush. The center color is the color that appears at the brush's center point.
old-location: gdiplus\_gdiplus_CLASS_PathGradientBrush_SetCenterColor_color_.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\classes\pathgradientbrushclass\pathgradientbrushmethods\setcentercolor.htm
ms.author: windowssdkdev
ms.date: 10/09/2018
ms.keywords: PathGradientBrush class [GDI+],SetCenterColor method, PathGradientBrush.SetCenterColor, PathGradientBrush::SetCenterColor, SetCenterColor, SetCenterColor method [GDI+], SetCenterColor method [GDI+],PathGradientBrush class, _gdiplus_CLASS_PathGradientBrush_SetCenterColor_color_, gdiplus._gdiplus_CLASS_PathGradientBrush_SetCenterColor_color_
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: gdipluspath.h
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
 - PathGradientBrush.SetCenterColor
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# PathGradientBrush::SetCenterColor


## -description


The <b>PathGradientBrush::SetCenterColor</b> method sets the center color of this path gradient brush. The center color is the color that appears at the brush's center point.


## -parameters




### -param color [in, ref]

Type: <b>const <a href="https://msdn.microsoft.com/dae648fd-1302-481e-9f5b-331a4c1b5e0d">Color</a></b>

Reference to a <a href="https://msdn.microsoft.com/dae648fd-1302-481e-9f5b-331a4c1b5e0d">Color</a> object that specifies the center color. 


## -returns



Type: <strong>Type: <b><a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a></b>
</strong>

If the method succeeds, it returns <b>Ok</b>, which is an element of the 
						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.

If the method fails, it returns one of the other elements of the 
						<a href="https://msdn.microsoft.com/035fb1bb-cdf3-47e5-a4c7-024598fa01a3">Status</a> enumeration.




## -remarks



By default the center point is the centroid of the brush's boundary path, but you can set the center point to any location inside or outside the path.


#### Examples



The following example creates a 
						<a href="https://msdn.microsoft.com/cac0a3ce-982e-4de5-a160-cb8a755beddd">PathGradientBrush</a>object based on an ellipse. The code calls the <b>PathGradientBrush::SetCenterColor</b> method of the 
						<b>PathGradientBrush</b>object to set the center color to blue. The 
						<a href="https://msdn.microsoft.com/80c24a7a-feed-40a3-bbdf-ff971e8aac68">PathGradientBrush::SetSurroundColors</a> method sets the color along the entire boundary to aqua. The 
						<a href="https://msdn.microsoft.com/91d3fc66-4c0d-4b44-beae-59f13b80483d">FillRectangle Methods</a> method uses the path gradient brush to paint a rectangle that contains the ellipse.

<div class="code"><span codelanguage="ManagedCPlusPlus"><table>
<tr>
<th>C++</th>
</tr>
<tr>
<td>
<pre>VOID Example_SetCenter(HDC hdc)
{
   Graphics graphics(hdc);

   // Create a path that consists of a single ellipse.
   GraphicsPath path;
   path.AddEllipse(0, 0, 200, 100);

   // Use the path to construct a brush.
   PathGradientBrush pthGrBrush(&amp;path);

   // Set the color at the center of the path to blue.
   pthGrBrush.SetCenterColor(Color(255, 0, 0, 255));

   // Set the color along the entire boundary of the path to aqua.
   Color colors[] = {Color(255, 0, 255, 255)};
   INT count = 1;
   pthGrBrush.SetSurroundColors(colors, &amp;count);

   graphics.FillRectangle(&amp;pthGrBrush, 0, 0, 300, 300); 
}</pre>
</td>
</tr>
</table></span></div>



## -see-also




<a href="https://msdn.microsoft.com/889558d5-9181-43ff-b862-e92966324208">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/dae648fd-1302-481e-9f5b-331a4c1b5e0d">Color</a>



<a href="https://msdn.microsoft.com/f6a8085c-3d6a-494f-a1ee-5fa96efb1aae">Creating a Path Gradient</a>



<a href="https://msdn.microsoft.com/7aa94b39-bd4c-4e66-b0dc-77f8953797b1">Filling a Shape with a Color Gradient</a>



<a href="https://msdn.microsoft.com/1072a5cc-4e82-41f4-aaad-5f90eb2cfa22">GraphicsPath</a>



<a href="https://msdn.microsoft.com/cac0a3ce-982e-4de5-a160-cb8a755beddd">PathGradientBrush</a>



<a href="https://msdn.microsoft.com/b5b79732-f89a-46fb-b7ac-2eb45f7d4f87">PathGradientBrush::GetCenterColor</a>



<a href="https://msdn.microsoft.com/6bd4993d-2401-4070-be0e-dbac684095d3">PathGradientBrush::GetCenterPoint Methods</a>



<a href="https://msdn.microsoft.com/41765887-b1de-4259-95af-a1ef8c84d01a">PathGradientBrush::SetCenterPoint Methods</a>
 

 


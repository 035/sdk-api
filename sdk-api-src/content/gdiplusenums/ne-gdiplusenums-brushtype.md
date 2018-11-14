---
UID: NE:gdiplusenums.BrushType
title: BrushType
author: windows-sdk-content
description: The BrushType enumeration indicates the type of brush. There are five types of brushes.
old-location: gdiplus\_gdiplus_ENUM_BrushType.htm
tech.root: gdiplus
ms.assetid: VS|gdicpp|~\gdiplus\gdiplusreference\enumerations\brushtype.htm
ms.author: windowssdkdev
ms.date: 11/09/2018
ms.keywords: BrushType, BrushType enumeration [GDI+], BrushTypeHatchFill, BrushTypeLinearGradient, BrushTypePathGradient, BrushTypeSolidColor, BrushTypeTextureFill, _gdiplus_ENUM_BrushType, gdiplus._gdiplus_ENUM_BrushType, gdiplusenums/BrushType, gdiplusenums/BrushTypeHatchFill, gdiplusenums/BrushTypeLinearGradient, gdiplusenums/BrushTypePathGradient, gdiplusenums/BrushTypeSolidColor, gdiplusenums/BrushTypeTextureFill
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: gdiplusenums.h
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
req.lib: 
req.dll: 
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Gdiplusenums.h
api_name:
 - BrushType
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
req.product: GDI+ 1.0
---

# BrushType enumeration


## -description


The <b>BrushType</b> enumeration indicates the type of brush. There are five types of brushes.


## -enum-fields




### -field BrushTypeSolidColor

Indicates a brush of type <a href="https://msdn.microsoft.com/8d5c8780-f03c-40b2-b237-e40121e3d6f6">SolidBrush</a>. A solid brush paints a single, constant color that can be opaque or transparent. 


### -field BrushTypeHatchFill

Indicates a brush of type <a href="https://msdn.microsoft.com/6e633cb2-8b0f-4b6a-95d8-f494d5f972eb">HatchBrush</a>. A hatch brush paints a background and paints, over that background, a pattern of lines, dots, dashes, squares, crosshatch, or some variation of these. The hatch brush consists of two colors: one for the background and one for the pattern over the background. The color of the background is called the 
				<i>background color</i>, and the color of the pattern is called the 
				<i>foreground color</i>. 


### -field BrushTypeTextureFill

Indicates a brush of type <a href="https://msdn.microsoft.com/4657ed8b-9cec-49ba-bf20-545bf3ee51f9">TextureBrush</a>. A texture brush paints an image. The image or 
				<i>texture</i> is either a portion of a specified image or a scaled version of a specified image. The type of image (metafile or nonmetafile) determines whether the texture is a portion of the image or a scaled version of the image. 


### -field BrushTypePathGradient

Indicates a brush of type <a href="https://msdn.microsoft.com/cac0a3ce-982e-4de5-a160-cb8a755beddd">PathGradientBrush</a>. A path gradient brush paints a color gradient in which the color changes from a center point outward to a boundary that is defined by a closed curve or path. The color gradient has one color at the center point and one or multiple colors at the boundary. 


### -field BrushTypeLinearGradient

Indicates a brush of type <a href="https://msdn.microsoft.com/43901cd3-b059-4830-9063-e8287899e18a">LinearGradientBrush</a>. A linear gradient brush paints a color gradient in which the color changes evenly from the starting boundary line of the linear gradient brush to the ending boundary line of the linear gradient brush. The boundary lines of a linear gradient brush are two parallel straight lines. The color gradient is perpendicular to the boundary lines of the linear gradient brush, changing gradually across the stroke from the starting boundary line to the ending boundary line. The color gradient has one color at the starting boundary line and another color at the ending boundary line. 


## -see-also




<a href="https://msdn.microsoft.com/889558d5-9181-43ff-b862-e92966324208">Brushes and Filled Shapes</a>



<a href="https://msdn.microsoft.com/6e633cb2-8b0f-4b6a-95d8-f494d5f972eb">HatchBrush</a>



<a href="https://msdn.microsoft.com/43901cd3-b059-4830-9063-e8287899e18a">LinearGradientBrush</a>



<a href="https://msdn.microsoft.com/cac0a3ce-982e-4de5-a160-cb8a755beddd">PathGradientBrush</a>



<a href="https://msdn.microsoft.com/8d5c8780-f03c-40b2-b237-e40121e3d6f6">SolidBrush</a>



<a href="https://msdn.microsoft.com/4657ed8b-9cec-49ba-bf20-545bf3ee51f9">TextureBrush</a>



<a href="https://msdn.microsoft.com/8ccf2c4a-6f99-465f-8adf-0f7fcd002f79">Using a Brush to Fill Shapes</a>
 

 


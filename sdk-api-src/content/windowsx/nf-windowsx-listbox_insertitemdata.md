---
UID: The unique id of the API.
title: The title of the API.
author: Authoring type of the API(ie windows-driver-content)
description: Description of API
old-location: 
old-project: 
ms.assetid: The MSDN ID of the API
ms.author: The Author of the API
ms.date: The date of API publishing
ms.keywords: 
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: The topic type of the API (ie enum)
req.header: The main header of the API
req.include-header: The included headers of the API
req.target-type: 
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
---

# ListBox_InsertItemData macro


## -description


Inserts item data to a list box at the specified location. You can use this macro or send the <a href="https://msdn.microsoft.com/dfaa742d-2f42-4485-aed5-cda8ca9ba66c">LB_INSERTSTRING</a> message explicitly.


## -parameters




### -param hwndCtl

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

A handle to the control.


### -param index

Type: <b>int</b>

The zero-based index in the list at which to insert the item data, or –1 to add it to the end of the list.


### -param data

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">LPARAM</a></b>

A pointer to the item data to insert.


## -remarks



Use this macro for a list box with an owner-drawn style but without the <a href="List_Box_Styles.htm">LBS_HASSTRINGS</a> style. For more information, see <a href="https://msdn.microsoft.com/dfaa742d-2f42-4485-aed5-cda8ca9ba66c">LB_INSERTSTRING</a>.
	




---
UID: NF:winuser.CharToOemBuffW
title: CharToOemBuffW function
author: windows-sdk-content
description: Translates a specified number of characters in a string into the OEM-defined character set.
old-location: menurc\chartooembuff.htm
tech.root: menurc
ms.assetid: VS|winui|~\winui\windowsuserinterface\resources\strings\stringreference\stringfunctions\chartooembuff.htm
ms.author: windowssdkdev
ms.date: 11/15/2018
ms.keywords: CharToOemBuff, CharToOemBuff function [Menus and Other Resources], CharToOemBuffA, CharToOemBuffW, _win32_CharToOemBuff, _win32_chartooembuff_cpp, menurc.chartooembuff, winui._win32_chartooembuff, winuser/CharToOemBuff, winuser/CharToOemBuffA, winuser/CharToOemBuffW
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: winuser.h
req.include-header: Windows.h
req.target-type: Windows
req.target-min-winverclnt: Windows 2000 Professional [desktop apps only]
req.target-min-winversvr: Windows 2000 Server [desktop apps only]
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: CharToOemBuffW (Unicode) and CharToOemBuffA (ANSI)
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: User32.lib
req.dll: User32.dll
req.irql: 
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - DllExport
api_location:
 - User32.dll
 - Ext-MS-Win-NTUser-chartranslation-l1-1-0.dll
api_name:
 - CharToOemBuff
 - CharToOemBuffA
 - CharToOemBuffW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- CharToOemBuffW
: 
---

# CharToOemBuffW function


## -description


Translates a specified number of characters in a string into the OEM-defined character set.


## -parameters




### -param lpszSrc [in]

Type: <b>LPCTSTR</b>

The null-terminated string to be translated.


### -param lpszDst [out]

Type: <b>LPSTR</b>

The buffer for the translated string. If the <b>CharToOemBuff</b> function is being used as an ANSI function, the string can be translated in place by setting the <i>lpszDst</i> parameter to the same address as the <i>lpszSrc</i> parameter. This cannot be done if <b>CharToOemBuff</b> is being used as a wide-character function. 


### -param cchDstLength [in]

Type: <b>DWORD</b>

The number of characters to translate in the string identified by the <i>lpszSrc</i> parameter.


## -returns



Type: <b>BOOL</b>

The return value is always nonzero except when you pass the same address to <i>lpszSrc</i> and <i>lpszDst</i> in the wide-character version of the function. In this case the function returns zero and <a href="https://msdn.microsoft.com/d852e148-985c-416f-a5a7-27b6914b45d4">GetLastError</a> returns <b>ERROR_INVALID_ADDRESS</b>.




## -remarks



Unlike the <a href="https://msdn.microsoft.com/66588b51-1673-4cb0-828f-9e00de4a622e">CharToOem</a> function, the <b>CharToOemBuff</b> function does not stop converting characters when it encounters a null character in the buffer pointed to by <i>lpszSrc</i>. The <b>CharToOemBuff</b> function converts all <i>cchDstLength</i> characters.




## -see-also




<a href="https://msdn.microsoft.com/66588b51-1673-4cb0-828f-9e00de4a622e">CharToOem</a>



<b>Conceptual</b>



<a href="https://msdn.microsoft.com/2336b758-7b57-44d2-b3ce-34054128a26d">OemToChar</a>



<a href="https://msdn.microsoft.com/17b01f13-6c09-43e2-984c-3b085f6b353f">OemToCharBuff</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/f2cb0888-b245-448c-9910-a634312aff67">Strings</a>
 

 


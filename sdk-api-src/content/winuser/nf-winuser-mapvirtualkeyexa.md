---
UID: NF:winuser.MapVirtualKeyExA
title: MapVirtualKeyExA function
author: windows-sdk-content
description: Translates (maps) a virtual-key code into a scan code or character value, or translates a scan code into a virtual-key code. The function translates the codes using the input language and an input locale identifier.
old-location: inputdev\mapvirtualkeyex.htm
tech.root: inputdev
ms.assetid: VS|winui|~\winui\windowsuserinterface\userinput\keyboardinput\keyboardinputreference\keyboardinputfunctions\mapvirtualkeyex.htm
ms.author: windowssdkdev
ms.date: 09/26/2018
ms.keywords: MAPVK_VK_TO_CHAR, MAPVK_VK_TO_VSC, MAPVK_VK_TO_VSC_EX, MAPVK_VSC_TO_VK, MAPVK_VSC_TO_VK_EX, MapVirtualKeyEx, MapVirtualKeyEx function [Keyboard and Mouse Input], MapVirtualKeyExA, MapVirtualKeyExW, _win32_MapVirtualKeyEx, _win32_mapvirtualkeyex_cpp, inputdev.mapvirtualkeyex, winui._win32_mapvirtualkeyex, winuser/MapVirtualKeyEx, winuser/MapVirtualKeyExA, winuser/MapVirtualKeyExW
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
req.unicode-ansi: MapVirtualKeyExW (Unicode) and MapVirtualKeyExA (ANSI)
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
 - Ext-MS-Win-NTUser-Keyboard-l1-1-0.dll
 - Ext-MS-Win-NTUser-Keyboard-l1-1-1.dll
 - api-ms-win-ntuser-ie-keyboard-l1-1-0.dll
 - ie_stubs.dll
 - ext-ms-win-ntuser-keyboard-l1-1-2.dll
 - Ext-MS-Win-NTUser-Keyboard-L1-2-0.dll
 - Ext-MS-Win-NTUser-Keyboard-L1-2-1.dll
 - Ext-MS-Win-NTUser-Keyboard-L1-3-0.dll
api_name:
 - MapVirtualKeyEx
 - MapVirtualKeyExA
 - MapVirtualKeyExW
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- 
: 
- MapVirtualKeyExA
: 
---

# MapVirtualKeyExA function


## -description


Translates (maps) a virtual-key code into a scan code or character value, or translates a scan code into a virtual-key code. The function translates the codes using the input language and an input locale identifier.


## -parameters




### -param uCode [in]

Type: <b>UINT</b>

The virtual-key code or scan code for a key. How this value is interpreted depends on the value of the <i>uMapType</i> parameter.

Starting with Windows Vista, the high byte of the <i>uCode</i> value can contain either 0xe0 or 0xe1 to specify the extended scan code.


### -param uMapType [in]

Type: <b>UINT</b>

The translation to perform. The value of this parameter depends on the value of the <i>uCode</i> parameter.

<table>
<tr>
<th>Value</th>
<th>Meaning</th>
</tr>
<tr>
<td width="40%"><a id="MAPVK_VK_TO_CHAR"></a><a id="mapvk_vk_to_char"></a><dl>
<dt><b>MAPVK_VK_TO_CHAR</b></dt>
<dt>2</dt>
</dl>
</td>
<td width="60%">
The <i>uCode</i> parameter is a virtual-key code and is translated into an unshifted character value in the low order word of the return value. Dead keys (diacritics) are indicated by setting the top bit of the return value. If there is no translation, the function returns 0.

</td>
</tr>
<tr>
<td width="40%"><a id="MAPVK_VK_TO_VSC"></a><a id="mapvk_vk_to_vsc"></a><dl>
<dt><b>MAPVK_VK_TO_VSC</b></dt>
<dt>0</dt>
</dl>
</td>
<td width="60%">
The <i>uCode</i> parameter is a virtual-key code and is translated into a scan code. If it is a virtual-key code that does not distinguish between left- and right-hand keys, the left-hand scan code is returned. If there is no translation, the function returns 0.

</td>
</tr>
<tr>
<td width="40%"><a id="MAPVK_VK_TO_VSC_EX"></a><a id="mapvk_vk_to_vsc_ex"></a><dl>
<dt><b>MAPVK_VK_TO_VSC_EX</b></dt>
<dt>4</dt>
</dl>
</td>
<td width="60%">
The <i>uCode</i> parameter is a virtual-key code and is translated into a scan code. If it is a virtual-key code that does not distinguish between left- and right-hand keys, the left-hand scan code is returned. If the scan code is an extended scan code, the high byte of the <i>uCode</i> value can contain either 0xe0 or 0xe1 to specify the extended scan code. If there is no translation, the function returns 0.

</td>
</tr>
<tr>
<td width="40%"><a id="MAPVK_VSC_TO_VK"></a><a id="mapvk_vsc_to_vk"></a><dl>
<dt><b>MAPVK_VSC_TO_VK</b></dt>
<dt>1</dt>
</dl>
</td>
<td width="60%">
The <i>uCode</i> parameter is a scan code and is translated into a virtual-key code that does not distinguish between left- and right-hand keys. If there is no translation, the function returns 0.

</td>
</tr>
<tr>
<td width="40%"><a id="MAPVK_VSC_TO_VK_EX"></a><a id="mapvk_vsc_to_vk_ex"></a><dl>
<dt><b>MAPVK_VSC_TO_VK_EX</b></dt>
<dt>3</dt>
</dl>
</td>
<td width="60%">
The <i>uCode</i> parameter is a scan code and is translated into a virtual-key code that distinguishes between left- and right-hand keys. If there is no translation, the function returns 0.

</td>
</tr>
</table>
 


### -param dwhkl [in, out, optional]

Type: <b>HKL</b>

Input locale identifier to use for translating the specified code. This parameter can be any input locale identifier previously returned by the <a href="https://msdn.microsoft.com/6e35847e-d641-4ff2-80b6-a5b5293ebbdc">LoadKeyboardLayout</a> function.


## -returns



Type: <b>UINT</b>

The return value is either a scan code, a virtual-key code, or a character value, depending on the value of <i>uCode</i> and <i>uMapType</i>. If there is no translation, the return value is zero.




## -remarks



The input locale identifier is a broader concept than a keyboard layout, since it can also encompass a speech-to-text converter, an Input Method Editor (IME), or any other form of input.

An application can use <b>MapVirtualKeyEx</b> to translate scan codes to the virtual-key code constants <b>VK_SHIFT</b>, <b>VK_CONTROL</b>, and <b>VK_MENU</b>, and vice versa. These translations do not distinguish between the left and right instances of the SHIFT, CTRL, or ALT keys.

An application can get the scan code corresponding to the left or right instance of one of these keys by calling <b>MapVirtualKeyEx</b> with <i>uCode</i> set to one of the following virtual-key code constants.

<ul>
<li><b>VK_LSHIFT</b></li>
<li><b>VK_RSHIFT</b></li>
<li><b>VK_LCONTROL</b></li>
<li><b>VK_RCONTROL</b></li>
<li><b>VK_LMENU</b></li>
<li><b>VK_RMENU</b></li>
</ul>
These left- and right-distinguishing constants are available to an application only through the <a href="https://msdn.microsoft.com/d6b31d2c-43b3-4502-a7ed-af564895f27e">GetKeyboardState</a>, <a href="https://msdn.microsoft.com/9c34dd1f-b423-4dcd-b29e-8bf64be57472">SetKeyboardState</a>, <a href="https://msdn.microsoft.com/edc449e4-f37d-4f2c-8add-45b905bd3326">GetAsyncKeyState</a>, <a href="https://msdn.microsoft.com/41c7bcc7-0a14-420c-b338-7ca13c95b7b8">GetKeyState</a>, <a href="https://msdn.microsoft.com/d287c66d-def1-4794-a95b-fa7c93e7bd35">MapVirtualKey</a>, and <b>MapVirtualKeyEx</b> functions. For list complete table of virtual key codes, see <a href="https://msdn.microsoft.com/fa8926ad-41b2-4164-9ba3-ae501fd0eef2">Virtual Key Codes</a>.




## -see-also




<b>Conceptual</b>



<a href="https://msdn.microsoft.com/edc449e4-f37d-4f2c-8add-45b905bd3326">GetAsyncKeyState</a>



<a href="https://msdn.microsoft.com/41c7bcc7-0a14-420c-b338-7ca13c95b7b8">GetKeyState</a>



<a href="https://msdn.microsoft.com/d6b31d2c-43b3-4502-a7ed-af564895f27e">GetKeyboardState</a>



<a href="https://msdn.microsoft.com/a3f6ac32-cde9-440d-bbde-0d76b4b5d4a4">Keyboard Input</a>



<a href="https://msdn.microsoft.com/6e35847e-d641-4ff2-80b6-a5b5293ebbdc">LoadKeyboardLayout</a>



<b>Reference</b>



<a href="https://msdn.microsoft.com/9c34dd1f-b423-4dcd-b29e-8bf64be57472">SetKeyboardState</a>
 

 


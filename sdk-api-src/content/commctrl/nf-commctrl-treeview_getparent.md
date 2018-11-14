---
UID: NF:commctrl.TreeView_GetParent
title: TreeView_GetParent macro
author: windows-sdk-content
description: Retrieves the parent item of the specified tree-view item. You can use this macro, or you can explicitly send the TVM_GETNEXTITEM message with the TVGN_PARENT flag.
old-location: controls\TreeView_GetParent.htm
tech.root: controls
ms.assetid: VS|Controls|~\controls\treeview\macros\treeview_getparent.htm
ms.author: windowssdkdev
ms.date: 11/02/2018
ms.keywords: TreeView_GetParent, TreeView_GetParent macro [Windows Controls], _win32_TreeView_GetParent, _win32_TreeView_GetParent_cpp, commctrl/TreeView_GetParent, controls.TreeView_GetParent, controls._win32_TreeView_GetParent
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: macro
req.header: commctrl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Windows Vista [desktop apps only]
req.target-min-winversvr: Windows Server 2003 [desktop apps only]
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
 - Commctrl.h
api_name:
 - TreeView_GetParent
product: Windows
targetos: Windows
req.typenames: 
req.redist: 
- apiref
: 
- HeaderDef
: 
- commctrl.h
: 
- TreeView_GetParent
: 
---

# TreeView_GetParent macro


## -description


Retrieves the parent item of the specified tree-view item. You can use this macro, or you can explicitly send the <a href="https://msdn.microsoft.com/505c713c-7728-4119-bc0e-482fe7e73193">TVM_GETNEXTITEM</a> message with the TVGN_PARENT flag. 


## -parameters




### -param hwnd

Type: <b><a href="https://msdn.microsoft.com/4553cafc-450e-4493-a4d4-cb6e2f274d46">HWND</a></b>

Handle to the tree-view control. 


### -param hitem

Type: <b>HTREEITEM</b>

Handle to an item. 


## -remarks



This macro will return <b>NULL</b> if the parent of the specified item is the root node of the tree.




## -see-also




<b>Reference</b>



<a href="https://msdn.microsoft.com/49eb25c4-52b3-4b3a-ae2f-433af9adf0d4">TreeView_GetChild</a>



<a href="https://msdn.microsoft.com/987d0d0f-eecf-4a6a-9340-64dd6ce1ac80">TreeView_GetNextItem</a>



<a href="https://msdn.microsoft.com/1fe480ea-dcb5-4d08-8eec-996f78757fda">TreeView_GetNextSibling</a>



<a href="https://msdn.microsoft.com/2f013ffb-43dd-460f-824a-36fb67639834">TreeView_GetPrevSibling</a>
 

 


---
UID: NF:windowsx.ScrollBar_SetPos
title: ScrollBar_SetPos macro (windowsx.h)
description: Sets the position of the scroll box (thumb) in the specified scroll bar and, if requested, redraws the scroll bar to reflect the new position of the scroll box. (ScrollBar_SetPos)
helpviewer_keywords: ["ScrollBar_SetPos","ScrollBar_SetPos macro [Windows Controls]","_win32_ScrollBar_SetPos","_win32_ScrollBar_SetPos_cpp","controls.ScrollBar_SetPos","controls._win32_ScrollBar_SetPos","windowsx/ScrollBar_SetPos"]
old-location: controls\ScrollBar_SetPos.htm
tech.root: Controls
ms.assetid: VS|Controls|~\controls\scrollbars\scrollbarreference\scrollbarmacros\scrollbar_setpos.htm
ms.date: 10/21/2024
ms.keywords: ScrollBar_SetPos, ScrollBar_SetPos macro [Windows Controls], _win32_ScrollBar_SetPos, _win32_ScrollBar_SetPos_cpp, controls.ScrollBar_SetPos, controls._win32_ScrollBar_SetPos, windowsx/ScrollBar_SetPos
req.header: windowsx.h
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
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - ScrollBar_SetPos
 - windowsx/ScrollBar_SetPos
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - Windowsx.h
api_name:
 - ScrollBar_SetPos
---

# ScrollBar_SetPos macro

## -syntax

```cpp
BOOL ScrollBar_SetPos(
   HWND hwndCtl,
   int  pos,
   BOOL fRedraw
);
```

## -returns

Type: **[BOOL](/windows/desktop/winprog/windows-data-types)**

See <b>SetScrollPos</b>.


## -description

Sets the position of the scroll box (thumb) in the specified scroll bar and, if requested, redraws the scroll bar to reflect the new position of the scroll box. 
        
<div class="alert"><b>Note</b>  This macro expands to a call to the <a href="/windows/desktop/api/winuser/nf-winuser-setscrollpos">SetScrollPos</a> function, which is deprecated. New applications should use the <a href="/windows/desktop/api/winuser/nf-winuser-setscrollinfo">SetScrollInfo</a> function.</div><div> </div>

## -parameters

### -param hwndCtl

Type: <b><a href="/windows/desktop/WinProg/windows-data-types">HWND</a></b>

A handle to the control.

### -param pos

Type: <b>int</b>

The new position of the scroll box.

### -param fRedraw

Type: <b><a href="/windows/desktop/WinProg/windows-data-types">BOOL</a></b>

<b>TRUE</b> to redraw the control; otherwise <b>FALSE</b>.

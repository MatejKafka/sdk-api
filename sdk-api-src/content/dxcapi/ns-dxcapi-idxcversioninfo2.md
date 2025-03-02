---
UID: NS:dxcapi.IDxcVersionInfo2
tech.root: direct3dhlsl
title: IDxcVersionInfo2
ms.date: 04/05/2023
targetos: Windows
description: Represents PDB version information.
prerelease: false
req.construct-type: structure
req.ddi-compliance: 
req.dll: 
req.header: dxcapi.h
req.include-header: 
req.kmdf-ver: 
req.lib: 
req.max-support: 
req.redist: 
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.target-type: 
req.typenames: 
typedef_isUnnamed: false
req.umdf-ver: 
req.unicode-ansi: 
topic_type:
 - apiref
api_type:
 - HeaderDef
api_location:
 - dxcapi.h
api_name:
 - IDxcVersionInfo2
f1_keywords:
 - IDxcVersionInfo2
 - dxcapi/IDxcVersionInfo2
dev_langs:
 - c++
helpviewer_keywords:
 - IDxcVersionInfo2
---

## -description

Represents PDB version information.

To obtain an instance of this interface, call [IDxcPdbUtils::GetVersionInfo](./nf-dxcapi-idxcpdbutils-getversioninfo.md) to obtain a **IDxcVersionInfo** interface, and then use **QueryInterface** to obtain an instance of this interface from it.

## -remarks

## -see-also

---
UID: NF:directxpackedvector.XMStoreShortN4
title: XMStoreShortN4 function (directxpackedvector.h)
description: Stores an XMVECTOR in an XMSHORTN4.
helpviewer_keywords: ["DirectX::PackedVector.XMStoreShortN4","XMStoreShortN4","XMStoreShortN4 method [DirectX Math Support APIs]","dxmath.xmstoreshortn4"]
old-location: dxmath\xmstoreshortn4.htm
tech.root: dxmath
ms.assetid: M:Microsoft.directx_sdk.storing.XMStoreShortN4(XMSHORTN4@,XMVECTOR)
ms.date: 12/05/2018
ms.keywords: DirectX::PackedVector.XMStoreShortN4, XMStoreShortN4, XMStoreShortN4 method [DirectX Math Support APIs], dxmath.xmstoreshortn4
req.header: directxpackedvector.h
req.include-header: DirectXPackedVector.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: DirectX::PackedVector
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
 - XMStoreShortN4
 - directxpackedvector/XMStoreShortN4
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - directxpackedvector.inl
api_name:
 - XMStoreShortN4
---

# XMStoreShortN4 function


## -description

Stores an <a href="https://docs.microsoft.com/windows/desktop/dxmath/xmvector-data-type">XMVECTOR</a> in an <a href="https://docs.microsoft.com/windows/desktop/api/directxpackedvector/ns-directxpackedvector-xmshortn4">XMSHORTN4</a>.

## -parameters

### -param pDestination [out]

Address at which to store the data.

### -param V [in]

Vector containing the data to store.

## -returns

None.

## -remarks

The following pseudocode demonstrates the operation of the function.


```
XMVECTOR N;	
static const XMVECTOR  Scale = {32767.0f, 32767.0f, 32767.0f, 32767.0f};

assert(pDestination);

N = XMVectorClamp(V, g_XMNegativeOne, g_XMOne);
N = XMVectorMultiply(N, Scale);
N = XMVectorRound(N);

pDestination->x = (int16_t)N.v[0];
pDestination->y = (int16_t)N.v[1];
pDestination->z = (int16_t)N.v[2];
pDestination->w = (int16_t)N.v[3];
```


<h3><a id="Platform_Requirements"></a><a id="platform_requirements"></a><a id="PLATFORM_REQUIREMENTS"></a>Platform Requirements</h3>
Microsoft Visual Studio 2010 or Microsoft Visual Studio 2012 with the Windows SDK for Windows 8. Supported for Win32 desktop apps, Windows Store apps, and Windows Phone 8 apps.

## -see-also

<a href="https://docs.microsoft.com/windows/desktop/dxmath/ovw-xnamath-reference-functions-storage">DirectXMath Library Vector Store Functions</a>


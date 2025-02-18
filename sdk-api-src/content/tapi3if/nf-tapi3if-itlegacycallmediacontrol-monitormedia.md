---
UID: NF:tapi3if.ITLegacyCallMediaControl.MonitorMedia
title: ITLegacyCallMediaControl::MonitorMedia (tapi3if.h)
description: The MonitorMedia method sets monitoring for a given media type on the current call.
helpviewer_keywords: ["ITLegacyCallMediaControl interface [TAPI 2.2]","MonitorMedia method","ITLegacyCallMediaControl.MonitorMedia","ITLegacyCallMediaControl::MonitorMedia","MonitorMedia","MonitorMedia method [TAPI 2.2]","MonitorMedia method [TAPI 2.2]","ITLegacyCallMediaControl interface","_tapi3_itlegacycallmediacontrol_monitormedia","tapi3.itlegacycallmediacontrol_monitormedia","tapi3if/ITLegacyCallMediaControl::MonitorMedia"]
old-location: tapi3\itlegacycallmediacontrol_monitormedia.htm
tech.root: tapi3
ms.assetid: 82efd729-fbbf-449f-a347-24bceada140c
ms.date: 12/05/2018
ms.keywords: ITLegacyCallMediaControl interface [TAPI 2.2],MonitorMedia method, ITLegacyCallMediaControl.MonitorMedia, ITLegacyCallMediaControl::MonitorMedia, MonitorMedia, MonitorMedia method [TAPI 2.2], MonitorMedia method [TAPI 2.2],ITLegacyCallMediaControl interface, _tapi3_itlegacycallmediacontrol_monitormedia, tapi3.itlegacycallmediacontrol_monitormedia, tapi3if/ITLegacyCallMediaControl::MonitorMedia
req.header: tapi3if.h
req.include-header: Tapi3.h
req.target-type: Windows
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
req.lib: Uuid.lib
req.dll: Tapi3.dll
req.irql: 
targetos: Windows
req.typenames: 
req.redist: 
ms.custom: 19H1
f1_keywords:
 - ITLegacyCallMediaControl::MonitorMedia
 - tapi3if/ITLegacyCallMediaControl::MonitorMedia
dev_langs:
 - c++
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - Tapi3.dll
api_name:
 - ITLegacyCallMediaControl.MonitorMedia
---

# ITLegacyCallMediaControl::MonitorMedia


## -description

The 
<b>MonitorMedia</b> method sets monitoring for a given media type on the current call. This method enables and disables the detection of media types (modes) on the specified call. When a media type is detected, a message is sent to the application. For more information, see 
<a href="https://docs.microsoft.com/windows/desktop/api/tapi/nf-tapi-linemonitormedia">lineMonitorMedia</a>.

## -parameters

### -param lMediaType [in]

Indicator of 
<a href="https://docs.microsoft.com/windows/desktop/Tapi/tapimediatype--constants">media type</a>.

## -returns

This method can return one of these values.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
Method succeeded.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_INVALIDARG</b></dt>
</dl>
</td>
<td width="60%">
The <i>lMediaType</i> parameter is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_FAIL</b></dt>
</dl>
</td>
<td width="60%">
The associated call object is not valid.

</td>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>E_OUTOFMEMORY</b></dt>
</dl>
</td>
<td width="60%">
Insufficient memory exists to perform the operation.

</td>
</tr>
</table>

## -see-also

<a href="https://docs.microsoft.com/windows/desktop/api/tapi3if/nn-tapi3if-itlegacyaddressmediacontrol">ITLegacyAddressMediaControl</a>



<a href="https://docs.microsoft.com/windows/desktop/api/tapi3if/nn-tapi3if-itlegacycallmediacontrol">ITLegacyCallMediaControl</a>


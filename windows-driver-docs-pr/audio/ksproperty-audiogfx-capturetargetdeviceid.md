---
title: KSPROPERTY\_AUDIOGFX\_CAPTURETARGETDEVICEID
description: The KSPROPERTY\_AUDIOGFX\_CAPTURETARGETDEVICEID property is used to inform a GFX filter of the Plug and Play device ID of the audio device that is the source of the capture stream.
ms.assetid: df4505c5-f9ff-4f8a-8521-90031c0b23e4
keywords: ["KSPROPERTY_AUDIOGFX_CAPTURETARGETDEVICEID Audio Devices"]
topic_type:
- apiref
api_name:
- KSPROPERTY_AUDIOGFX_CAPTURETARGETDEVICEID
api_location:
- Ksmedia.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
ms.localizationpriority: medium
---

# KSPROPERTY\_AUDIOGFX\_CAPTURETARGETDEVICEID


The KSPROPERTY\_AUDIOGFX\_CAPTURETARGETDEVICEID property is used to inform a GFX filter of the Plug and Play device ID of the audio device that is the source of the capture stream.

## <span id="ddk_ksproperty_audiogfx_capturetargetdeviceid_ks"></span><span id="DDK_KSPROPERTY_AUDIOGFX_CAPTURETARGETDEVICEID_KS"></span>


### <span id="Usage_Summary_Table"></span><span id="usage_summary_table"></span><span id="USAGE_SUMMARY_TABLE"></span>Usage Summary Table

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Get</th>
<th align="left">Set</th>
<th align="left">Target</th>
<th align="left">Property descriptor type</th>
<th align="left">Property value type</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>No</p></td>
<td align="left"><p>Yes</p></td>
<td align="left"><p>Filter</p></td>
<td align="left"><p>[<strong>KSPROPERTY</strong>](https://msdn.microsoft.com/library/windows/hardware/ff564262)</p></td>
<td align="left"><p>WCHAR array</p></td>
</tr>
</tbody>
</table>

 

The property value (operation data) is a WCHAR array that contains the device ID. The device ID is a null-terminated string of Unicode characters.

### <span id="Return_Value"></span><span id="return_value"></span><span id="RETURN_VALUE"></span>Return Value

A KSPROPERTY\_AUDIOGFX\_CAPTURETARGETDEVICEID property request returns STATUS\_SUCCESS to indicate that it has completed successfully. Otherwise, the request returns an appropriate error status code.

Remarks
-------

The target for this set-only property request is a GFX filter that is configured for use as either a capture- or render/capture-GFX filter.

To determine the size of the buffer needed to hold the property value, see [Basic Support Queries for Audio Properties](https://msdn.microsoft.com/library/windows/hardware/ff536225).

For additional information about GFX filters and device IDs, see [GFX Filters](https://msdn.microsoft.com/library/windows/hardware/ff536403) and [Device Identification Strings](https://msdn.microsoft.com/library/windows/hardware/ff541224).

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Header</p></td>
<td align="left">Ksmedia.h (include Ksmedia.h)</td>
</tr>
</tbody>
</table>

## <span id="see_also"></span>See also


[**KSPROPERTY**](https://msdn.microsoft.com/library/windows/hardware/ff564262)

 

 







---
title: RequestSendAndForgetNoFormatting rule (kmdf)
description: The RequestSendAndForgetNoFormatting rule verifies that the driver doesn't format a request using the I/O target formatting functions before sending it to an I/O target with the send option WDF\_REQUEST\_SEND\_OPTION\_SEND\_AND\_FORGET.
ms.assetid: C98C0C04-3345-49D6-9669-40D1A4F9CDBB
ms.author: windowsdriverdev
ms.date: 05/21/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
keywords: ["RequestSendAndForgetNoFormatting rule (kmdf)"]
topic_type:
- apiref
api_name:
- RequestSendAndForgetNoFormatting
api_type:
- NA
ms.localizationpriority: medium
---

# RequestSendAndForgetNoFormatting rule (kmdf)


The **RequestSendAndForgetNoFormatting** rule verifies that the driver doesn't format a request using the I/O target formatting functions before sending it to an I/O target with the send option WDF\_REQUEST\_SEND\_OPTION\_SEND\_AND\_FORGET.

|              |      |
|--------------|------|
| Driver model | KMDF |

How to test
-----------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">At compile time</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Run [Static Driver Verifier](https://msdn.microsoft.com/library/windows/hardware/ff552808) and specify the <strong>RequestSendAndForgetNoFormatting</strong> rule.</p>
Use the following steps to run an analysis of your code:
<ol>
<li>[Prepare your code (use role type declarations).](https://msdn.microsoft.com/library/windows/hardware/hh454281#preparing-your-source-code)</li>
<li>[Run Static Driver Verifier.](https://msdn.microsoft.com/library/windows/hardware/hh454281#running-static-driver-verifier)</li>
<li>[View and analyze the results.](https://msdn.microsoft.com/library/windows/hardware/hh454281#viewing-and-analyzing-the-results)</li>
</ol>
<p>For more information, see [Using Static Driver Verifier to Find Defects in Drivers](https://msdn.microsoft.com/library/windows/hardware/hh454281).</p></td>
</tr>
</tbody>
</table>

Applies to
----------

[**WdfIoTargetFormatRequestForInternalIoctl**](https://msdn.microsoft.com/library/windows/hardware/ff548595)
[**WdfIoTargetFormatRequestForInternalIoctlOthers**](https://msdn.microsoft.com/library/windows/hardware/ff548599)
[**WdfIoTargetFormatRequestForIoctl**](https://msdn.microsoft.com/library/windows/hardware/ff548604)
[**WdfIoTargetFormatRequestForRead**](https://msdn.microsoft.com/library/windows/hardware/ff548612)
[**WdfIoTargetFormatRequestForWrite**](https://msdn.microsoft.com/library/windows/hardware/ff548620)
[**WdfRequestSend**](https://msdn.microsoft.com/library/windows/hardware/ff550027)
[**WdfUsbTargetDeviceFormatRequestForControlTransfer**](https://msdn.microsoft.com/library/windows/hardware/ff550082)
[**WdfUsbTargetDeviceFormatRequestForCyclePort**](https://msdn.microsoft.com/library/windows/hardware/ff550084)
[**WdfUsbTargetDeviceFormatRequestForString**](https://msdn.microsoft.com/library/windows/hardware/ff550086)
[**WdfUsbTargetDeviceFormatRequestForUrb**](https://msdn.microsoft.com/library/windows/hardware/ff550088)
[**WdfUsbTargetPipeFormatRequestForAbort**](https://msdn.microsoft.com/library/windows/hardware/ff551132)
[**WdfUsbTargetPipeFormatRequestForRead**](https://msdn.microsoft.com/library/windows/hardware/ff551136)
[**WdfUsbTargetPipeFormatRequestForReset**](https://msdn.microsoft.com/library/windows/hardware/ff551138)
[**WdfUsbTargetPipeFormatRequestForUrb**](https://msdn.microsoft.com/library/windows/hardware/ff551139)
[**WdfUsbTargetPipeFormatRequestForWrite**](https://msdn.microsoft.com/library/windows/hardware/ff551141)
 

 






---
title: PcTimedWaveRtStreamSetState rule (audio)
description: The PcTimedWaveRtStreamSetState rule specifies that a ProtCls miniport driver makes state transitions through IMiniportWaveRTStream SetState within the required time.
ms.assetid: D49869E0-9108-460B-8FA3-4FD99C3EA81E
keywords: ["PcTimedWaveRtStreamSetState rule (audio)"]
topic_type:
- apiref
api_name:
- PcTimedWaveRtStreamSetState
api_type:
- NA
---

# PcTimedWaveRtStreamSetState rule (audio)


The PcTimedWaveRtStreamSetState rule specifies that a ProtCls miniport driver makes state transitions through [**IMiniportWaveRTStream::SetState**](https://msdn.microsoft.com/library/windows/hardware/ff536756) within the required time.

|              |       |
|--------------|-------|
| Driver model | Audio |

|                                   |                                                                                                                                       |
|-----------------------------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Bug check(s) found with this rule | [**Bug Check 0xC4: DRIVER\_VERIFIER\_DETECTED\_VIOLATION**](https://msdn.microsoft.com/library/windows/hardware/ff560187) (0x00072001) |

How to test
-----------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">At run time</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>To verify this rule, open a Command Prompt window. Enter a Driver Verifier command and specify <strong>/domain audio</strong>.</p>
<p>For example:</p>
<p><strong>verifier /domain audio</strong> [<em>options</em>] <strong>/driver</strong> <em>&lt;yourdriver&gt;</em></p>
<p>For more information, see [Driver Verifier](https://msdn.microsoft.com/library/windows/hardware/ff545448).</p></td>
</tr>
</tbody>
</table>

 

 

 






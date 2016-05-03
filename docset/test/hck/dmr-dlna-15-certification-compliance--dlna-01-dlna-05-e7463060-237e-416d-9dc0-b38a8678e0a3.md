---
author: joshbax-msft
title: DMR DLNA 1.5 Certification Compliance (DLNA-01 DLNA-05)
description: DMR DLNA 1.5 Certification Compliance (DLNA-01 DLNA-05)
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 07aae316-68f5-42f5-8f5a-924df6cad198
---

# DMR DLNA 1.5 Certification Compliance (DLNA-01 DLNA-05)


This test verifies that the digital media renderer (DMR) device has been certified by the Digital Living Network Alliance (DLNA-01) and that the certification is comprised of the required DLNA device roles (DLNA-05, DLNA-10). As part of configuring the DMR tests in the Windows Hardware Certification Kit, you will be asked to enter the DLNA certificate ID.

**DLNA-01** (Applies to A/V DMR and Audio DMR)

A Digital Media Renderer must demonstrate compliance with the DLNA protocols using one of the following alternatives:

-   The DMR passes the DLNA Certification Program and obtains a DLNA certificate.

-   The DMR uses an OEM reference design (hardware/software) that has already passed the DLNA Certification Program and has obtained a DLNA certificate (as long as the DMR complies with Windows Hardware Certification policies on devices covered by the same certificate).

-   The DMR uses middleware from an independent software provider. The middleware has passed the DLNA Certification Program and has obtained a DLNA certificate.

If the device implements multiple network interfaces, such as Ethernet and Wireless Ethernet, the DLNA Certificate must indicate a satisfactory evaluation using all interfaces.

If the device also implements a DMP, the device must demonstrate compliance with the DLNA protocols for the DMP class using one of the alternatives mentioned above.

**DLNA-05** (Applies to A/V DMR)

An A/V DMR is a renderer that plays images, audio, and videos. The DLNA certification for an A/V DMR must include the Image Class, the Audio Class, and the A/V Class.

**DLNA-10** (Applies to Audio DMR)

An Audio DMR is a renderer that plays audio but not video. The DLNA certification for an Audio DMR must include the Audio Class. If an Audio DMR plays images, the DLNA certification for this Audio DMR must include the Image Class.

## Test details


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Associated requirements</strong></p></td>
<td><p>Device.Media.DMR.Base.DLNA15CertificationCompliance</p>
<p>[See the device hardware requirements.](http://go.microsoft.com/fwlink/p/?linkid=254483)</p></td>
</tr>
<tr class="even">
<td><p><strong>Platforms</strong></p></td>
<td><p>Windows 7 (x64) Windows 7 (x86) Windows 8 (x64) Windows 8 (x86) Windows 8.1 x64 Windows 8.1 x86</p></td>
</tr>
<tr class="odd">
<td><p><strong>Expected run time</strong></p></td>
<td><p>~2 minutes</p></td>
</tr>
<tr class="even">
<td><p><strong>Categories</strong></p></td>
<td><p>Certification</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>Manual</p></td>
</tr>
</tbody>
</table>

 

## Running the test


In addition, you must have obtained a DLNA certificate ID for the device.

## Troubleshooting


For troubleshooting information, see [Troubleshooting Device.Media Testing](troubleshooting-devicemedia-testing.md).

## More information


### Parameters

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parameter</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>WDKData_DeviceUUID</p></td>
<td><p>The Device ID</p></td>
</tr>
<tr class="even">
<td><p>WDKData_DLNAID</p></td>
<td><p>The ID of the DLNA certificate.</p></td>
</tr>
</tbody>
</table>

 

### Command syntax

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Command option</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>NetMediaLogoTests.exe NETMEDIA_0003 /dmrID=[Query WDKData_DeviceUUID] /dlnaID=[WDKData_DLNAID]</strong></p></td>
<td><p>Runs the test.</p></td>
</tr>
</tbody>
</table>

 

### File list

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>File</th>
<th>Location</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>NetMediaLogoTests.exe</p></td>
<td><p><em>&lt;testbinroot&gt;</em>\nttest\multimediatest\sharing\netmedialogotests\</p></td>
</tr>
</tbody>
</table>

 

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bp_hck\p_hck%5D:%20DMR%20DLNA%201.5%20Certification%20Compliance%20%28DLNA-01%20DLNA-05%29%20%20RELEASE:%20%284/27/2016%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




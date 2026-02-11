# XR Systems

This page provides a brief introduction to the typical hardware and software components of an XR system. Modern XR systems are unified sets of hardware, with supporting software, which are used to provide end users with the capability of accessing immersive media content like XR-enabled 3D software and 360 video. Here we focus primarily on contemporary, off-the-shelf XR systems, which are frequently used by creators.

Common components of XR systems include:

* [**Head-mounted display**](./) **(HMD)** which is placed over the users head, providing the screens which create the visual illusion of being in a virtual environment.
* **Human Input Device (HID)** which allows the user to interact with elements of the virtual experience (e.g. by pressing buttons or moving a joystick).
* **Tracking system** which translates user movement in the physical environment into movement in the virtual environment using camera and/or sensor data. In practice this is often integrated, at least partially, into HMD and/or HID devices
* **Computer system** to run the XR software, which can be integrated into the headset (e.g. in the Oculus Quest series) or run standalone (for tethered headsets like the Oculus Rift S or Valve Index).
* [**Supporting software**](/broken/pages/-MhEDeOt4_pd5lLf9Blz) which provides interfaces between these hardware components and XR software.

These components can be integrated to varying degrees (e.g. an HMD can contain a tracking system), as described in the subsections below.

The commercial marketplace has strongly influenced the development of XR systems since the early 2010's when a "second wave" of immersive technologies started. Most companies produce tiered feature sets at varying price points (e.g. the Meta Quest 3 and Meta Quest 3S). Releases of product models might follow incremental improvements in technology, resulting in very similar systems with only one or two differences between them — or releases could represent a big jump in technology or hardware design from year to year. It can be challenging to identify defining features and technical specifications for a given XR system because of advertising styles (many hard-to-prove claims are made) and the proprietary, competitive nature of development.

### Head-Mounted Displays

A Head-Mounted Display (HMD) is a display device, worn on the head or as part of a helmet, that mounts either a single screen in front of both of the users eyes (monocular HMD) or a separate screens in front of each eye (binocular HMD).&#x20;

The simplest and cheapest type of XR system uses a handheld mobile phone mount, with embedded lenses that help the user focus on the close range screen. This creates means that the full (or most) of the visual range of the user is taken up by the screen content, which supports the feeling of immersion in the virtual environment. The internal gyroscope is used to support [3DoF movement](../../getting-started/initial-assessment.md#interactivity). Google Cardboard (pictured below) is an example of a handheld device of this type. This was a low cost solution made of cardboard and containing plastic lenses, released in 2014 and now discontinued.&#x20;

<figure><img src="../../.gitbook/assets/image (3).png" alt="" width="375"><figcaption><p>Google Cardboard VR headset, released in 2014, shown assembled and with an iPhone 6s in the visor slot.</p></figcaption></figure>

Exceeding these low cost system in features, complexity and comfort are more sophisticated Head-Mounted Display (HMD) devices, that are hands-free and provide increased immersion. HMDs can be tethered systems (e.g. the Oculus Rift series, pictured below), which are connected to a computer using cabling running from the HMD. This allows them to offer better performance in terms of graphics and location processing, as the computer is able to handle this work.&#x20;

<figure><img src="../../.gitbook/assets/image (4).png" alt="" width="375"><figcaption><p>The Meta Quest 3, released in 2023, is an example of a standalone headset which houses a built-in computer.</p></figcaption></figure>

Standalone HMDs (e.g. Meta Quest series, pictured below, VIVE Focus series) contain built in computers which run the XR content, eliminating the need for cabling running to an external computer. This offers the user greater freedom of motion and tend to be less expensive overall, at the cost of reduced processing power.

Detailed and regularly updated information about the properties of XR HMDs are available on [XinReality](https://vrarwiki.com/wiki/Virtual_Reality_Devices) and [Wikipedia](https://en.wikipedia.org/wiki/Comparison_of_virtual_reality_headsets). The spreadsheet[^1] linked below, created by sasha arden, gathers information about popular XR systems from various sources, for the purpose of conveniently identifying their key features. It could be useful for considering compatibility in the case of a potential hardware replacement or migration. For example if the XR content uses 6DoF interactivity, an XR system that is only capable of supporting 3DoF would not be suitable.&#x20;

{% embed url="https://docs.google.com/spreadsheets/d/1DkoRL4VxXeFyuoj-ybToMn4jrzSrStAPjgX9JXGZKs8/edit?usp=sharing" %}
_XR Systems Comparison (In Progress)_ \[2021-22] compiled by sasha arden.
{% endembed %}

### Tracking Systems

Further interactivity and immersion is achieved with tracking systems, which provide input for the XR content and/or information about the user's position in space. Tracking systems can be built into the HMD (e.g. Meta Quest series) using cameras or additional hardware incorporating sensors is used alongside an HMD (e.g. Oculus Rift 'Constellation' or Valve Index 'Base Stations').&#x20;

## Supporting Software

Communication between XR hardware and an XR application (be it 3D software or a 360 degree video player) is contingent on supporting software. Support for a suitable runtime (or runtime standard) is built into the software supplied by manufacturers and support is added to XR appication by their developers.&#x20;

Until 2019 there was no standardisation of XR runtimes, which resulted in poor compatibility between software and hardware, making changes to hardware difficult. The situation has dramatically improved with the arrival of a standard, called [OpenXR](openxr.md), which helps ensure that devices and software speak the same language. For more information about OpenXR, and guidance on compatibility across hardware and software platforms, see the [OpenXR page](openxr.md).

Supporting software is required to connect XR software (e.g. a VR application or 360 video player) to XR hardware. This is typically a software package provided by the manufacturer of an XR hardware system. This may include a user-facing application with a storefront for purchasing content (e.g. Steam or Oculus) but also includes back-end software components which serve a technical role.

The most important component of this package from a preservation perspective is an _XR runtime_, which provides an API and driver to support an interface between XR applications and XR devices. It can also provide features that modify the behaviour of XR applications (e.g. improving performance of image quality). Examples include the Oculus runtime and the SteamVR runtime. An XR runtime can provide XR applications with a variety of interfaces with which to interact with them, which might conform to a standards such as [OpenXR](openxr.md) or OpenVR.&#x20;

<table><thead><tr><th width="161">Runtime Name</th><th width="159">OpenXR Support</th><th width="153">OS Support</th><th>Download Packages</th></tr></thead><tbody><tr><td>Oculus Runtime</td><td>Yes</td><td><p>Android</p><p>Windows 10/11</p></td><td>Current version only downloadable through Oculus client. Legacy versions available on <a href="https://developer.oculus.com/downloads/package/oculus-runtime-for-windows/">https://developer.oculus.com/downloads/package/oculus-runtime-for-windows/</a></td></tr><tr><td>SteamVR</td><td>Yes</td><td><p>Windows 7 (SP1)</p><p>Windows 8.1 </p><p>Windows 10/11</p></td><td>Can only be downloaded through Steam (see <a href="archiving-an-xr-runtime.md">Archiving XR Runtimes</a>).</td></tr><tr><td>Monado</td><td>Yes</td><td><p>Android</p><p>Linux<br>Windows 10/11</p></td><td>Source code available from <a href="https://gitlab.freedesktop.org/monado/monado">GitLab</a>, build packages available for Debian and Ubuntu only. </td></tr></tbody></table>

[^1]: The spreadsheet was last updated in 2022 and is out of date. For up to date information, refer to the XinReality and Wikipedia sources linked above. If anyone is interested in updating this table, let us know!

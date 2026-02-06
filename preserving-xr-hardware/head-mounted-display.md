# XR Systems

## Introduction to Modern XR Systems

Modern XR systems are unified sets of hardware, with supporting software, which are used to provide end users with the capability of accessing immersive media content like XR-enabled 3D software and 360 video. Common components of XR systems include:

* [**Head-mounted display**](head-mounted-display.md) **(HMD)** which is placed over the users head, providing the screens which create the visual illusion of being in a virtual environment.
* **Human Input Device (HID)** which allows the user to interact with elements of the virtual experience (e.g. by pressing buttons or moving a joystick).
* **Tracking system** which translates user movement in the physical environment into movement in the virtual environment using camera and/or sensor data. In practice this is often integrated, at least partially, into HMD and/or HID devices
* **Computer system** to run the XR software, which can be integrated into the headset (e.g. in the Oculus Quest series) or run standalone (for tethered headsets like the Oculus Rift S or Valve Index).
* [**Supporting software**](xr-runtimes/) which provides interfaces between these hardware components and XR software.

### Head-Mounted Displays

The simplest type of XR system uses a handheld mobile phone mount with lenses that help to focus on the screen content and create the illusion of an immersive view. Google Cardboard is an example of such a handheld device of this type. The next step in features and complexity involves a more sophisticated [head-mounted display (HMD)](head-mounted-display.md) that is hands-free and provides a better illusion of immersion.&#x20;

Further interactivity and immersion is achieved with tracking systems, which provide input for the XR content and/or information about the user's position in space. Tracking systems can be built into the HMD (e.g. Oculus Quest series) or hardware incorporating sensors is used along with an HMD (e.g. Oculus Rift or HTC Vive).&#x20;

Another category among XR systems is standalone types and tethered types. Standalone HMDs (e.g. Oculus Quest, HTC Vive Focus) offer greater freedom of motion and are less expensive overall, while tethered systems (e.g. Oculus Rift S, HTC Vive Pro) use a connected computer to offer better performance in terms of graphics and location processing.&#x20;

The commercial marketplace has strongly influenced development of XR systems since the early 2010's when a "second wave" of immersive technologies started. Most companies produce tiered feature sets at varying price points. Releases of product models might follow incremental improvements in technology, resulting in very similar systems with only one or two differences between them -- or releases could represent a big jump in technology or hardware design from year to year. It can be challenging to identify defining features and technical specifications for a given XR system because of advertising styles (many hard-to-prove claims are made) and the proprietary, competitive nature of development.

### Comparison of XR HMDs

A head-mounted display (HMD) is a display device, worn on the head or as part of a helmet, that mounts either a single screen in front of both of the users eyes (monocular HMD) or a separate screen in front of each eye (binocular HMD). An extensive summary of the properties of VR HMDs is available on the [XinReality](https://xinreality.com/wiki/Virtual_Reality_Devices) wiki or on [Wikipedia](https://en.wikipedia.org/wiki/Comparison_of_virtual_reality_headsets). HMDs are generally either "tethered" (such as Oculus Rift) to a PC that monitors tracking and undertakes the rendering, or "untethered" (such as Oculus Quest) where the unit is standalone.&#x20;

The table below is meant to gather information for the purpose of identifying the features of popular XR systems. It could be useful for considering compatibility in the case of a potential hardware replacement or migration. For example if the XR content uses 6DOF interactivity, an XR system that is only capable of supporting 3DOF would not be suitable.

{% embed url="https://docs.google.com/spreadsheets/d/1DkoRL4VxXeFyuoj-ybToMn4jrzSrStAPjgX9JXGZKs8/edit?usp=sharing" %}
_XR Systems Comparison (In Progress)_ \[2021-22] compiled by sasha arden.
{% endembed %}

### HMD-Runtime Compatibility

<table data-header-hidden><thead><tr><th width="328"> HMD Name</th><th> Supported Runtimes</th></tr></thead><tbody><tr><td> <strong>HMD Name</strong></td><td> <strong>Supported Runtimes</strong></td></tr><tr><td>Oculus Rift CV1</td><td>Oculus Runtime; SteamVR</td></tr><tr><td>HTC Vive</td><td>SteamVR; Oculus Runtime (via <a href="https://github.com/LibreVR/Revive">Revive</a>)</td></tr></tbody></table>

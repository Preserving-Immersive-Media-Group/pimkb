# Archiving an XR Runtime

{% hint style="warning" %}
This page has been deprecated is it no longer represents our recommend approach. We would instead recommend migrating XR projects to [OpenXR](openxr.md), which provides a degree of backwards compatibility.
{% endhint %}

This page describes the process for extracting an XR runtime as a contained unit of software, so that it can be archived independently of a computer system. XR runtime are often distributed using front-end tools that carry out downloading and installation in the background (e.g. SteamVR is downloaded through Steam). This makes it harder to extract and archive them for reuse in the future. This page describes the process of extracting different XR runtimes for independent archiving.&#x20;

## Oculus (Windows)

Legacy Oculus Runtime 0.8.0 (dating from 2017) is currently available to download from the Oculus website: [https://developer.oculus.com/downloads/package/oculus-runtime-for-windows/](https://developer.oculus.com/downloads/package/oculus-runtime-for-windows/).

For later versions you are dependent on the [Oculus Rift software](https://www.oculus.com/rift/setup/?locale=en_GB) to install and manage the runtime. After installation, the runtime can be found in C:\Program Files\Oculus. Testing is needed to ascertain whether this directory can be copied to a new machine.

## SteamVR (Windows)

These instructions are adapted from Valve's [guidelines for offline installation](https://partner.steamgames.com/doc/features/steamvr/enterprise) of SteamVR. While this method allows you to extract a standalone copy of the SteamVR runtime, the version available through Steam cannot be controlled.&#x20;

1\. Either a) Install and open the [Steam Client](https://store.steampowered.com/about/) on a PC with full internet access or b) Access a computer which already has the appropriate version of Steam installed.&#x20;

2\. In the Steam Client, open the Library section and find the part of it labeled "Tools".

3\. Find the entry "SteamVR" and install it.

4\. Right-click on the entry "SteamVR" and in the resulting popup menu click on the entry "Properties".

![](../../.gitbook/assets/Archiving_SteamVR_1.png)

5\. A new window with multiple tabs will open. Select the tab "LOCAL FILES" and click on the button labeled "BROWSE LOCAL FILES".

![](../../.gitbook/assets/Archiving_SteamVR_2.png)

6\. The directory containing the SteamVR Runtime will open. Copying this entire directory will capture the files required to run SteamVR on another computer. From this directory, SteamVR can be launched by running the "vrstartup.exe" executable file in "\SteamVR\bin\win64".

![](../../.gitbook/assets/Archiving_SteamVR_3.png)

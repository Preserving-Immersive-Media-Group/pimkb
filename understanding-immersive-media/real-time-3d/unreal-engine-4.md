---
description: >-
  This page is designed to help you understand what Unreal Engine 4 is and how
  it can be used by creators.
---

# Unreal Engine 4

Unreal Engine 4 (UE4) is a real-time 3D engine developed by Epic Games. The first version of Unreal Engine was created during the development of the 1998 game Unreal, at which point Epic Game started licencing the engine to other developers. Version 4.0 was released in 2014, and has been followed by 27 subversions (the latest is 4.27). Unreal Engine 5, announced in 2020, is expected to supersede UE4 at some point in the near future. UE4 is not an open-source engine (see the EULA), but the engine source code is freely available via their GitHub repository.&#x20;

![ A sample project viewed in the Unreal Engine 4 editor (version 4.27).](../../.gitbook/assets/UE4\_27\_Editor.png)

## Anatomy of a UE4 Project

A UE4 project consists of a collection of files and folders conforming to a well defined structure. A project folder typically contains the following at the top-level:&#x20;

* **Binaries**: If the project has been compiled for a specific platform, this contains the files produced.&#x20;
* **Build:**&#x20;
* **Config**: Contains project settings stored in plain text files with the .ini extension.
* **Content**: Contains the maps, assets (e.g. 3D models, materials, blueprints) and other custom content used by the project, including any third-party packages downloaded from the Unreal Marketplace.&#x20;
* **DerivedDataCache** and **Intermediate**: Contain temporary files generated during the build process (e.g. shader compilation).
* **Saved**: Contains saved data created by the editor as it runs, including autosaves, crash reports and logs.
* **A .uproject file**: The project file with which the project can be launched. Actually a json file containing structured information describing the project, including the UE4 version, enabled plugins and target platforms.&#x20;

## Export Formats

When an asset is imported to Unreal Engine 4 it is converted to the UE4 UASSET (.uasset) format. This format is not well documented, although there is some partial reverse engineering work [here](http://wiki.xentax.com/index.php/Unreal\_Engine\_4\_UASSET). An UASSET can re-exported from the engine in a variety of formats depending on the asset type. To do so, you need to right click on the asset in the Content Browser, and navigate to Asset Actions -> Export.&#x20;

The information below was derived from testing in Unreal Engine 4.27.&#x20;

### 3D Models (Static)

| Format                   | Includes Material? | Nodes                                                                                  |
| ------------------------ | ------------------ | -------------------------------------------------------------------------------------- |
| FBX                      | Yes                | Can export to 2011, 2012, 2013, 2014, 2016, 2018, 2019, 2020 versions of the FBX spec. |
| OBJ                      | No                 |                                                                                        |
| Unreal object text .copy | No                 | Identical to .t3d                                                                      |
| Unreal object text .t3d  | No                 | Identical to .copy                                                                     |

## Anatomy of a UE4 Build

Dependent on whether Development or Shipping is selected prior to build, and other packaging options in UE4.&#x20;

## Anatomy of a UE4 Project

| UE4 Version | Target Platform | Dependencies                                                                                           |
| ----------- | --------------- | ------------------------------------------------------------------------------------------------------ |
| 4.27        | Linux           | [clang-11.0.1-based](https://cdn.unrealengine.com/CrossToolchain\_Linux/v19\_clang-11.0.1-centos7.exe) |
|             |                 |                                                                                                        |
|             |                 |                                                                                                        |

## UE4 Resources

* Epic Game, Unreal Engine 4.27 Glossary, URL: [https://docs.unrealengine.com/4.27/en-US/Basics/Glossary/](https://docs.unrealengine.com/4.27/en-US/Basics/Glossary/)
* David Lightbown, 2018, _Classic Tools Retrospective: Tim Sweeney on the first version of the Unreal Editor_. URL: [https://web.archive.org/web/20180823012812/https://www.gamasutra.com/blogs/DavidLightbown/20180109/309414/Classic\_Tools\_Retrospective\_Tim\_Sweeney\_on\_the\_first\_version\_of\_the\_Unreal\_Editor.php](https://web.archive.org/web/20180823012812/https://www.gamasutra.com/blogs/DavidLightbown/20180109/309414/Classic\_Tools\_Retrospective\_Tim\_Sweeney\_on\_the\_first\_version\_of\_the\_Unreal\_Editor.php)
*


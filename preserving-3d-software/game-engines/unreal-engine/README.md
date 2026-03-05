# Unreal Engine

[Unreal Engine](https://www.unrealengine.com/) is a series of game engines developed by Epic Games. The first version of Unreal Engine was created during the development of the 1998 game Unreal, at which point Epic Games started licencing the engine to other developers. Version 4.0 was released in 2014, and followed by 27 subversions. Unreal Engine 4 has now been superseded by Unreal Engine 5 and will no longer receive updates —  the final version released was 4.27. Projects can be [migrated from 4 to 5](https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-5-migration-guide) but manual migration of some elements may be required.

![A simple 3D scene open in the Unreal Engine 4.27 editor.](../../../.gitbook/assets/UE4_27_Interface.png)

This page is designed to help you understand the two major modern versions of Unreal Engine, 4 and 5, how they can be used by creators to develop 3D software and what your prospects are for the long-term preservation of an Unreal Engine project.

## Anatomy of a Unreal Engine Project

In general terms, an Unreal Engine project is the collection of custom code and data assets that are needed to build a specific project. By opening a .uproject file in the correct version of the Unreal Engine editor, the project can be loaded, examined and built. A project is analogous to source code, while a build is an executable application that can be run on any suitable computer.&#x20;

Behind the scenes, a Unreal Engine 4 and 5 projects consists of a collection of files and folders conforming to a well defined structure. A project folder typically contains the following at the top-level (more detail in the [Unreal Engine docs](https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-directory-structure)):&#x20;

* **Binaries**: If the project has been compiled for a specific platform, this contains the files produced.&#x20;
* **Build:** Contains files required to build the project for different platforms.&#x20;
* **Config**: Contains project settings stored in plain text files with the .ini extension.
* **Content**: Contains the maps, assets (e.g. 3D models, materials, blueprints) and other custom content used by the project, including any third-party packages downloaded from the Unreal Marketplace.&#x20;
* **DerivedDataCache** and **Intermediate**: Contain temporary files generated during the build process (e.g. shader compilation).
* **Saved**: Contains saved data created by the editor as it runs, including autosaves, crash reports and logs.
* **A .uproject file**: The project file with which the project can be launched. Actually a JSON file containing structured information describing the project, including the Unreal Engine version, enabled plugins and target platforms.

## Anatomy of a Unreal Engine Build

A built Unreal Engine applications consists of set of files and folders that allow the software to be run on a suitable host computer — usually targeting a specific platform like Windows or Linux.&#x20;

Though limited information can be gleaned from the packaged data and executable files, examining them can provide clues as to how the software was created. These include:&#x20;

* **An executable file** used to start the application.
* **/Engine folder** containing third-party libraries.
* **/**_**ProjectName**_**&#x20;folder** containing the full executable code, packed data (.pak files), configuration files (.ini) and logs.&#x20;

Some elements/features are dependent on whether the Development or Shipping option is selected prior to build, and other packaging options in the editor.&#x20;

## Preservation Considerations

### Overview

* Has been updated an average of four times per year since first release in 2014.&#x20;
  * Updates can result in deprecation or removal of features, or incompatibility with plugins — no Long-Term Support releases.
  * Migration from Unreal Engine 4 to 5 is relatively straightforward.
* Free source code access via GitHub repository (note that the Unreal Engine [EULA](https://www.unrealengine.com/en-US/eula/unreal) applies).
* Royalty payments only required with high product revenues, so unlikely to impact cultural heritage context.
* Situation regarding transfer of third-party licenced content (purchased from the Fab marketplace or equivalent) is unclear based on wording of Licence Agreement.&#x20;
* For custom C++ projects Visual Studio, dependencies are difficult to manage from an archival perspective as they depend on an opaque 'behind-the-scenes' installer provided by Microsoft.
* Transforms imported assets to the poorly documented internal format (.uasset). More work is required to understand whether this is used as a container format and whether changes occur during transformation.&#x20;
* [Texture compression](https://dev.epicgames.com/community/learning/tutorials/ry2D/reducing-package-sizes-with-oodle-compression) during build packaging can be used to reduce application size but is switched off by default.&#x20;

### Access and Licencing

<table><thead><tr><th width="269.9114802487602">Criteria</th><th width="470.7333577473958">Assessment</th></tr></thead><tbody><tr><td><strong>Source code access</strong></td><td>Public source code access although access to private GitHub repository needs to be requested. Not open source per se, released under the <a href="https://www.unrealengine.com/en-US/eula/unreal">Unreal Engine EULA</a>. Seems accommodating to preservation use case, but use must abide by EULA (e.g. no redistribution of engine source code). </td></tr><tr><td><strong>Licencing</strong></td><td>Engine use governed by <a href="https://www.unrealengine.com/en-US/eula/unreal">Unreal Engine EULA</a> and licenced third-party content by <a href="https://www.unrealengine.com/en-US/eula/content">Epic Content License Agreement</a>. Users to pay a 5% royalty to Epic Games if product revenues exceed $1,000,000 USD. </td></tr><tr><td><strong>Availability of old versions</strong></td><td>Oldest version available is 4.0.2 (released 28 March 2014) via Epic Games Launcher or GitHub.</td></tr></tbody></table>

### Export Formats

When an asset is imported to Unreal Engine 4/5 it is converted to the UASSET (.uasset) format. This format is not well documented, although there has been some [community reverse engineering work](http://wiki.xentax.com/index.php/Unreal_Engine_4_UASSET). A UASSET can be re-exported from the engine in a variety of formats depending on the asset type. To do so, you need to right click on the asset in the Content Browser, and navigate to Asset Actions -> Export.&#x20;

#### 3D Models (Static) Export Formats

The information below was derived from testing with a 3D model in Unreal Engine 4.27. Note that it is simply a list of the export formats _available_ and exports have not been tested against original import format.&#x20;

| Format                   | Includes Material? | Notes                                                                                  |
| ------------------------ | ------------------ | -------------------------------------------------------------------------------------- |
| FBX                      | Yes                | Can export to 2011, 2012, 2013, 2014, 2016, 2018, 2019, 2020 versions of the FBX spec. |
| OBJ                      | No                 |                                                                                        |
| Unreal object text .copy | No                 | Identical to .t3d                                                                      |
| Unreal object text .t3d  | No                 | Identical to .copy                                                                     |

### Game Dependencies

Windows applications created using the Unreal Engine editor have a set of dependencies similar to the editor. These are automatically packaged with an application when built from the editor, and are installed when the application is run by an installer program called 'UEPrereqSetup\_x64.exe' or similar. This can be located in the application directory: \[UEGameRootLocation]\Engine\Extras\Redist\en-us

### Editor Dependencies

To run the editor on **Windows 10 or 11**, a set of Microsoft .NET, Visual C++ and DirectX dependencies must be installed. Epic Games Launcher automatically runs a dependency installer when the engine is installed (called 'UEPrereqSetup\_x64.exe', 'UEPrereqSetup\_x86.exe' or similar), which selects the appropriate dependencies based on Windows version.&#x20;

Manually installing these is required if a different method of installation is used (e.g. copying the engine binaries onto the system). The manual installer can be located within the Engine directory: \[UE4EditorRootLocation]\Engine\Extras\Redist\en-us

There is also a version of the editor [available for Linux](https://www.unrealengine.com/en-US/linux). Operating system and Linux Kernel and glibc dependencies vary with version and can be loacted in the [specific engine versions doc](https://dev.epicgames.com/documentation/en-us/unreal-engine/linux-development-requirements-for-unreal-engine).

#### Build Dependencies

These dependencies are required to build software from the Windows version of the Unreal Engine editor, for the specific platforms noted.&#x20;

| Target Platform                    | Dependencies                                                                                                                                                                                                                                                                                                                                                            |
| ---------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Linux                              | clang for Linux (version depends on engine version: [https://docs.unrealengine.com/4.27/en-US/SharingAndReleasing/Linux/NativeToolchain/](https://docs.unrealengine.com/4.27/en-US/SharingAndReleasing/Linux/NativeToolchain/))                                                                                                                                         |
| Linux (cross-compile from Windows) | clang for Windows (version depends on engine version: [https://docs.unrealengine.com/4.27/en-US/SharingAndReleasing/Linux/AdvancedLinuxDeveloper/LinuxCrossCompileLegacy/](https://docs.unrealengine.com/4.27/en-US/SharingAndReleasing/Linux/AdvancedLinuxDeveloper/LinuxCrossCompileLegacy/))                                                                         |
| Windows                            | Visual Studio required for projects with code modification (version depends on engine version): [https://docs.unrealengine.com/5.0/en-US/setting-up-visual-studio-development-environment-for-cplusplus-projects-in-unreal-engine/](https://docs.unrealengine.com/5.0/en-US/setting-up-visual-studio-development-environment-for-cplusplus-projects-in-unreal-engine/)) |
| MacOS                              | ?                                                                                                                                                                                                                                                                                                                                                                       |

## Further Reading

* Epic Games, _**Unreal Engine Terminology**._ URL: [https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-terminology](https://dev.epicgames.com/documentation/en-us/unreal-engine/unreal-engine-terminology)
* David Lightbown, 2018, _**Classic Tools Retrospective: Tim Sweeney on the first version of the Unreal Editor**_. URL: [https://web.archive.org/web/20180823012812/https://www.gamasutra.com/blogs/DavidLightbown/20180109/309414/Classic\_Tools\_Retrospective\_Tim\_Sweeney\_on\_the\_first\_version\_of\_the\_Unreal\_Editor.php](https://web.archive.org/web/20180823012812/https://www.gamasutra.com/blogs/DavidLightbown/20180109/309414/Classic_Tools_Retrospective_Tim_Sweeney_on_the_first_version_of_the_Unreal_Editor.php)
* _**Unreal Engine Modding Tools**_. URL: [https://github.com/Buckminsterfullerene02/UE-Modding-Tools](https://github.com/Buckminsterfullerene02/UE-Modding-Tools)


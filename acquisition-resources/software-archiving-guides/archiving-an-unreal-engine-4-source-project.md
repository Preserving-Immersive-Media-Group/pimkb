---
description: >-
  This page describes the process for archiving an Unreal Engine 4 project and
  its dependencies, so that it can be archived independently of a computer
  system.
---

# Archiving an Unreal Engine 4 Source Project

One way of preparing for the preservation of software made in Unreal Engine 4 (UE4), is to archive the project files used to create it. While it is the executable form of the software (or 'build') which is used to run it, archiving the source form of the software opens up more preservation options such as:

* Creation of new builds which support different platforms and environments;
* Incremental migration to new versions of Unreal Engine 4;
* Migration to a new engine should this become necessary.
* Additionally, source materials can contain rich technical history and support an understanding of how the software was developed.&#x20;

As a rule of thumb, you want to have all the materials required to repeated the process of building the software. To build an Unreal Engine 4 project, you need the following components:

* ****[**Project folder**](archiving-an-unreal-engine-4-source-project.md#project-folder): the collection of custom Unreal Engine 4 content and project files;
* ****[**Engine binaries**](archiving-an-unreal-engine-4-source-project.md#engine-binaries): the editor software which allows you to open the project;
* ****[**Dependencies**](archiving-an-unreal-engine-4-source-project.md#dependencies): any additional software not included with the engine binaries by default e.g. plugins, libraries.

A sensible approach is therefore to archive all these components either independently or in the form of a disk image. Each component type, including how you can locate it, is described in detail below.&#x20;

## Project Folder

An Unreal Engine 4 project folder is a collection of files conforming to a specific directory structure — more information on this format can be found in our introduction to [Unreal Engine 4](../../understanding-immersive-media/game-engines/unreal-engine-4.md).&#x20;

The archive this, the supplier will need to send you a copy of this complete directory. The contents of this directory should look something like the screenshot below:&#x20;

![An example UE4 4.27 project folder.](../../.gitbook/assets/UE4\_ProjectDir.png)

One interesting thing to note is that this can include assets and other materials that are not used by the built application. This can make the project files larger, but also provides historical insight into the way it was created. If the creator of the project files offer to 'clean them up' before supplying them, you may wish to advise them against that.&#x20;

Project files can include hundreds or even thousands of files, so as a final step you may wish to ZIP them for convenience and reduced stored size.&#x20;

## Engine Binaries and Source Code

### Engine Binaries

To open an Unreal Engine 4 project you need an appropriate version of the Unreal Engine 4 editor. To avoid errors, you should use the editor version in which the project original developed. If you use a newer version, Unreal Engine will present a warning and give you a choice of whether to proceed or not. There is a chance you can open the project successfully, but doing so may break or change things, so do so very carefully and always _using a duplicate copy_.&#x20;

You can download prebuilt UE4 binaries using the [Epic Games Launcher](https://www.epicgames.com/store/en-US/download). Once installed, the engine version can be located in your UE4 install directory and zipped for archiving.&#x20;

Alternatively, you can build binaries from the [source code on GitHub](https://github.com/EpicGames/UnrealEngine) (this is a private repository and you will need to request access prior to use). See also the Binary Builder tool [https://github.com/ryanjon2040/Unreal-Binary-Builder](https://github.com/ryanjon2040/Unreal-Binary-Builder).

### Source Code

If the project involves a modified version of UE4, you will also need to archive a copy of the source code. Archiving the source code of the engine version used can also be a generally useful thing to have, as it can hold useful information for future preservation work.&#x20;

For a project using a modified source code, the creator should be able to supply this or advise on where it can be found. For unmodified UE4 source code, this can be pulled from the Unreal Engine repository on GitHub: [https://github.com/EpicGames/UnrealEngine](https://github.com/EpicGames/UnrealEngine). This is a private repository, so you will need to request access and link to an Epic Games account before being able to access it — see the [official instructions](https://docs.unrealengine.com/4.27/en-US/ProgrammingAndScripting/ProgrammingWithCPP/DownloadingSourceCode/).&#x20;

## Dependencies

Sometimes additional dependencies are required to open or build a UE4 project successfully.&#x20;

### Unreal Engine 4 plugins

Plugins are extensions to Unreal Engine 4's functionality. They can be installed from the within the engine or manually. There are two default locations for plugins:&#x20;

* Unreal Engine install location: /\[UE4 Root]/Engine/Plugins/\[Plugin Name]/
* Project folder: /\[Project Root]/Plugins/\[Plugin Name]/

You need to make sure that any required plugins have been installed and archived with either the project files or engine binaries.&#x20;

### C++ projects

If a UE4 project involves custom C++ code, you will need to install the appropriate version of Microsoft Visual Studio (e.g. 4.27 requires Visual Studio 2019 to build such project for Windows).&#x20;

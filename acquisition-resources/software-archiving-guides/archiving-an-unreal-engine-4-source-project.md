---
description: >-
  This page describes the process for archiving an Unreal Engine 4 project and
  its dependencies, so that it can be archived independently of a computer
  system.
---

# Archiving an Unreal Engine 4 Source Project

One way of preparing for the preservation of an application made in Unreal Engine 4 (UE4), is to archive the project used to create it.&#x20;

Executable software is created from an Unreal Engine 4 project by building an application that supports the target platform. By archiving an Unreal Engine 4 project, we aim to gather together all the materials required to carry out to repeat this build process. This opens up options for incremental migration to new versions of Unreal Engine, and the modification of code to support other hardware and software platforms.

To build an Unreal Engine 4 project, you need the following components:

* ****[**Project folder**](archiving-an-unreal-engine-4-source-project.md#project-folder): the collection of custom Unreal Engine 4 content and project files
* ****[**Engine binaries**](archiving-an-unreal-engine-4-source-project.md#engine-binaries): the editor software which allows you to open the project
* ****[**Dependencies**](archiving-an-unreal-engine-4-source-project.md#dependencies): any additional software not included with the engine binaries by default e.g. plugins, libraries

## Project Folder

An Unreal Engine 4 project folder is a collection of files conforming to a specific directory structure — more information on this format can be found in our introduction to [Unreal Engine 4](../../understanding-immersive-media/game-engines/unreal-engine-4.md).&#x20;

The archive this, the supplier will need to send you a copy of this complete directory. The contents of this directory should look something like the screenshot below:&#x20;

![An example UE4 4.27 project folder.](../../.gitbook/assets/UE4\_ProjectDir.png)

One interesting thing to note is that this can include assets and other materials that are not used by the built application.&#x20;

## Engine Binaries

To open an Unreal Engine 4 project you need an appropriate version of the Unreal Engine 4 editor. To avoid errors, you should use the editor version with which it the project was original developed. If you don't use this version, Unreal Engine will throw up a warning. There is a chance you can open the project successfully, but doing so may break or change things, so do so very carefully and _using a duplicate copy_.&#x20;

You can download prebuilt UE4 binaries using the [Epic Games Launcher](https://www.epicgames.com/store/en-US/download). Alternatively, you can build binaries from the source code on GitHub. See Binary Builder [https://github.com/ryanjon2040/Unreal-Binary-Builder](https://github.com/ryanjon2040/Unreal-Binary-Builder)

## Dependencies

Sometimes additional dependencies are used within the project or in order to build the application. These can include:&#x20;

* Unreal Engine 4 plugins
* Build dependencies (e.g. 4.27 requires Visual Studio 2019 to build for Windows)

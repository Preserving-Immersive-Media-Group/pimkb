---
description: >-
  This page describes the process for archiving a Unity 5 project and its
  dependencies on Windows, so that it can be preserved independently of a
  specific computer system.
---

# Archiving a Unity 5 Source Project

{% hint style="warning" %}
Work in progress!
{% endhint %}

One way of preparing for the preservation of an application made in Unity 5, is to archive the project files associated with it. Executable software is created from a Unity project by exporting an application that supports the target platform. By archiving an Unity project, we aim to gather together all the materials required to carry out to repeat this build process. This opens up options for incremental migration to new versions of Unity, and the modification of code to support other hardware and software platforms.

To build an Unity project, you need the following components, guidance on the archiving of which is provided on this page:&#x20;

* [Project folder:](archiving-a-unity-5-source-project.md#project-folder) the collection of custom Unity content and project files
* [Unity Editor](archiving-a-unity-5-source-project.md#engine-binaries): software which allows you to open and edit a Unity project folder
* [Dependencies](archiving-a-unity-5-source-project.md#dependencies): any additional software not included with the engine binaries or project by default e.g. libraries, modules

## Project Folder

\#

## Editor and Modules

The Unity Editor software can be installed using the Unity Hub software or from the intallers distributed via the [Unity Download Archive](https://unity3d.com/get-unity/download/archive).&#x20;

Before proceeding, you will need to identify the version of the Unity Editor the project was created with. To do so, navigate to the ProjectSettings folder within the project folder and open the file named ProjectVersion.txt (tested in 2018.3.9).&#x20;

### Using Unity Hub

1\. Install Unity Hub on a suitable computer and navigate to the Installs tab.&#x20;

![](../../.gitbook/assets/Archiving\_Unity5\_1.png)

2\. Click Install Editor and select the appropriate editor version. If the appropriate version is not available, you will need to install it use the Unity Download Archive method.&#x20;

![](<../../.gitbook/assets/Archiving Unity5\_2.png>)

You may also wish to install additional modules to improve build support.&#x20;

3\. Return to the previous Installs tab, click on the cog icon next to the Editor entry you wish to archive, and click on Show in Explorer.&#x20;

![](../../.gitbook/assets/Archiving\_Unity5\_3.png)

4\. In the Window which opens, you will be looking inside the application directory for the Unity Editor version. This folder can be archived and used to access the Editor independently of the Unity Hub installer.&#x20;

![](../../.gitbook/assets/Archiving\_Unity5\_4.png)

### Using Unity Download Archive



## Dependencies

There are two common ways of extending the functionality of Unity which you may find have been used: Modules and Packages.&#x20;

Modules extend core features, and includes options to build for non-Windows platforms. Unfortunately, if any non-standard modules have been used by the project your only option is to use the Unity Hub application to download and install these.&#x20;

Packages are handled by the Unity package manager module and are included in the project folder once they have been added.&#x20;

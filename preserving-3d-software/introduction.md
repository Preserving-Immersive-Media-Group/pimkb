# Introduction

Software can be used to generate a moving image sequence in real-time from 3D data sources. As frames are generated in real-time, this can be dynamic and/or interactive. This can be contrasted with video, where frames are encoded and played back linearly.

Existing software frameworks and tools are typically used as a starting point for development of 3D software, from which a distributable form of the software is generated. Development for desktop or mobile applications is typically using a [game engine](game-engines/). This can result in builds supporting different platforms e.g. desktop, mobile, web. Development for the web may involve the use of web frameworks like [Three.js](https://threejs.org/) and [A-Frame](https://aframe.io/).

## Assessing 3D Software

[**3D Software**](introduction.md) involves the use of software to dynamically generate a moving image sequence from 3D data and code. The real-time nature of the process means that the moving image sequence can be dynamic and responsive to user interaction. In practice, the technologies used here are often very similar to those involved in the creation of video games e.g. game engines, 3D modelling.&#x20;

Assessing 3D software involves identifying how it was made and how it can be accessed:&#x20;

* What **tools** were used in its creation and why were these chosen? e.g. [game engines](game-engines/), development frameworks, version control
* If a [**game engine**](game-engines/) was used:&#x20;
  * Is the specific engine **version** important?&#x20;
  * Was the engine **modified** in any way? e.g. plugins, rebuilt from source
  * Is the game engine (and any external dependencies required to run it) still **accessible and supported** by developer?&#x20;
  *    Can executable software still be **built from engine project** in a contemporary computing environment? This may take some effort to achieve but is a very valuable learning experience and indicates you have everything you need to maintain the software.
* What kinds of **asset** were used? e.g. custom made, third-party licenced
  * What **tools** were used to create the assets? e.g. 3D modelling, texturing, photogrammetry, animation/rigging
* How were any **audio** elements designed? Is sound dynamically triggered or from linear playback source?
* How **compatible** is the software with contemporary XR platforms? This will depend on how support has been built into the software during creation and how it has been distributed/displayed in the past e.g.
  * Was the software developed to run on a specific **computing platform?** e.g. Windows PC, Mac OS, Android, web platforms (A-Frame, Three.js) etc.
  * Was the software developed to run with a specific **XR hardware platform**? e.g. Oculus, SteamVR etc.
  * Does it make use of any external resources? e.g. additional software (e.g. Max); resources accessed via the internet etc.
* Are **source materials** available and how complex would these be to meaningfully preserve?&#x20;
  * What tools are needed to **build** the project from source materials as a standalone app/executable/webpage?&#x20;
  * Could source materials be **modified** to update the software?&#x20;
* Has **documentation of the experience** been supplied? If not, can it be created? e.g. fixed-perspective video capture, 360-degree video capture, installation photographs/video

## Acquisition Checklist

The following measures can help support long-term access to 3D software and prepare for future preservation interventions:

* Archive a copy of the **executable software** (ideally supporting as many operating systems and XR runtimes as possible).
* Identify, gather and test the **dependencies required to access the executable software** (e.g. operating systems, libraries, XR runtime, drivers).
* Archive a copy of the **source materials** (be it code or an engine project) and dependencies required to build the project — see [Software Archiving Guides](introduction.md).
* Identify, gather and test **dependencies required to access source materials**.
* Source or create **documentation** of the software running.

## **Further Reading**

[US Library of Congress Recommended Formats Statement: Software and Video Games](https://www.loc.gov/preservation/resources/rfs/software-videogames.html)

[Preserving 3D. Data Type Series. Artefactual Systems and the Digital Preservation Coalition. July 2021](http://doi.org/10.7207/twgn21-14)

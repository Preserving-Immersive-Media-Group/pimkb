# Preservation Strategies

XR content is highly dependent on specific hardware, particularly the HMD with its sensors, optics and electronics. Unfortunately, any single XR hardware system can be expected to eventually failure, particularly with regular use. Furthermore, the rapid obsolescence of these technologies is likely to eventually render them unrepairable and unreplaceable. Preservation strategies are applied to XR content to maintain access, despite these challenges, and so guide it into the future.&#x20;

## Preparation

In order to select and successfully apply a preservation strategy, you need to understand what it is you are trying to preserve. In an ideal world, full functionality and the same look and feel would be a preservation goal. However, in the real world technical limitations and limited resources may apply. From the outset of any interventive preservation work, stakeholders need to agree on acceptable degrees of loss or change to the artwork and develop the preservation strategy accordingly.&#x20;

A good starting point for this is our [initial assessment](../getting-started/initial-assessment.md) page. Working through these questions, ideally in consultation with the stakeholders of the XR material, you are aiming to identify:

* Which components or characteristics of the software are core to the XR experience? e.g. functionality, look and feel, user experience, quantitative / technical parameters; physical integrity.
* Which are variable or less important? Perfect replication may not be necessary to realise the XR experience authentically.
* Are they measurable or documentable in some way? Documentation can be very helpful as a reference for transmitting these characteristics e.g.
  * [Videos](video-documentation.md) and images of the work running.
  * A testing protocol which can help to verify different behaviours of the software, after changes are made. For example, applying a particular input and comparing the output to a documented reference.
  * Quantitative and technical parameters (e.g. framerate, frametime, display resolution) can be useful when assessing video or sound quality.&#x20;

This approach will help you determine what can and cannot change during the implementation of a preservation strategy, and develop a framework by which you can assess the success of a particular strategy. It is possible that compromises will have to be accepted because of financial or technical limitations. Therefore, applying a documentation strategy (see sub-section below) can complement one which priorities technical intervention.

Another consideration in developing a preservation strategy is its sustainability. If possible, a preservation strategy should _reduce_ dependencies and _stabilise_ the software so that the frequency interventive preservation measures is reduced. One way to make XR software more widely compatible is to make it hardware-independent. Currently, this goal is best supported by building in [OpenXR](../preserving-xr-hardware/head-mounted-display/openxr.md) support, a widely-adopted open standard for XR software. This maximises options in terms of switching to different XR hardware.

### Preservation Preparedness Checklist

The following measures, presented in order of increasing ambition, will help support long-term access to 3D software and prepare for future preservation interventions:

⭐ **First Steps:**&#x20;

* Archive a copy of the executable software.
* Source or create documentation of the software running.

🌟 **Next Level:**&#x20;

* Identify, gather and test the dependencies required to access the executable software (e.g. operating systems, libraries, XR runtime, drivers).&#x20;
  * In practice, this may be best created as a disk image, potentially created from the storage media of a tested computer system.
* Archive a copy of the source materials (be it purely code or a game engine project).

🌠 **Gold Standard:**&#x20;

* Identify, gather and test dependencies required to access and build source materials.
* If built in a game engine, consider migrating the source project to the latest release (ideally a Long-Term Support release, if available).
* Create and test builds supporting as many operating systems as possible — see [List of Engines](game-engines/#list-of-engines) for build support per engine.
* If not already present, add support for the [OpenXR standard](../preserving-xr-hardware/head-mounted-display/openxr.md) (e.g. via a game engine plugin or modifications to the source code) and test this new build.

## Documentation Strategies

A game engine can be used to output a 360 degree video, which can be preserved independently of the software as a video. **Capturing** the game engine output in this way is a type of **documentation** strategy. A 360 degree video is much easier to preserve than a game engine project with all its software dependencies. In addition, it does not depend on any specific XR hardware for continued access. To output a 360 degree video, usually the game project is necessary as most tools target specific game engine editors. However, it might be possible to capture the output from running the executable using [specific tools](video-documentation.md).&#x20;

[arden](https://www.tate.org.uk/documents/1793/Augmenting_Our_Approach_to_Preservation.pdf) (2022) advocates for the inside-out documentation approach, where the impact that the experience has on the user is central. This kind of documentation can become more relevant than the technical documentation of the artwork, if the functionality of the artwork cannot be preserved due to technical or financial constraints. This approach to documentation is practiced in performance art where the video documentation of the performance can replace the actual performance (for instance, Charlotte Moore performing Nam June Paik's TV cello in 1976).

However, if the capturing strategy is applied to interactive XR experiences, where the experience reacts to user input (other than the head movement), capturing the output leads to a total loss of that functionality. If this is not acceptable, the game engine project must be migrated to a version that supports newer XR hardware&#x20;

## Migration Strategies

A **migration strategy** involves updating the source code/project to run on newer computer or XR hardware. This requires access to the game engine source code/project (not just the executable) as well as the game engine editor software.&#x20;

Different approaches to migration can be taken e.g.

* Updating the game engine project to the newest LTS[^1] game engine version, and build the project for the newest runtime of the same headset brand.&#x20;
*   Updating the game engine project to the newest LTS[^2] game engine version and compiling the project for the OpenXR runtime. OpenXR has open specifications and "aims to

    to standardize the connections between VR applications and VR runtimes, and VR runtimes and VR hardware". Hence, after this migration, the risk that the game engine project cannot be transferred to a newer runtime is smaller than if exporting it for a proprietary runtime (Ensom and McConchie, Preserving Virtual Reality Works, [https://zenodo.org/records/5274102](https://zenodo.org/records/5274102), p. 11).

### Migration Case Studies

Case study applying an incremental migration strategy: LIMA (2021). _A Practical Research into Preservation Strategies for VR artworks on the basis of Justin Zijlstra’s 100 Jaar Vrouwenkiesrecht_. URL: [https://www.li-ma.nl/lima/article/preserving-vr-artworks](https://www.li-ma.nl/lima/article/preserving-vr-artworks)

## Emulation Strategies

An **emulation strategy** (and allied virtualization strategy) involves using a contemporary computer system to simulate a historical computer system. If there is only an executable, and the source code/project is not available, emulation can become an especially important preservation strategy for 3D software. Through emulation, the software environment is preserved as a whole, including the 3D software and any dependencies (e.g. the [XR runtime](../preserving-xr-hardware/head-mounted-display/#xr-runtime)).&#x20;

Emulation is mentioned at the end of this list, as it is often of rather limited use in the case of XR material. Gaining access to [XR hardware](/broken/pages/vvgkxh3hGQcJK7lb6Jmr) (e.g. an HMD) from an emulated environment has not been successfully achieved (or at least, documented) in a preservation context, as far as we are aware. However, emulation can be a more viable option if there is no [HMD](../preserving-xr-hardware/head-mounted-display/#head-mounted-displays) used, but other immersive displayed equipment (e.g. video projectors or monitors) are used instead.&#x20;



[^1]: LTS = Long-term-support, which means about 2 years

[^2]: &#x20;Long-Term Support, usually meaning about 2 years

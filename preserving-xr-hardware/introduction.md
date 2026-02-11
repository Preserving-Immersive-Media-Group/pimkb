# Introduction

**XR hardware** are the physical, hardware components used to access XR content. Contemporary XR hardware typically consists of a set of interconnected off-the-shelf hardware and software components, which we will refer to as an [XR system](head-mounted-display/).&#x20;

## Assessing XR Hardware

To start developing a preservation plan for XR hardware, begin by assessing characteristics of the hardware that the experience/content you wish to preserve depends on. Consider the following prompts:

* What kind of **computer system** is needed to run the software?
  * How flexible is the specification of the hardware?&#x20;
  * Is a **dedicated** [**GPU**](#user-content-fn-1)[^1] required? If so, does it require one with a specific feature set?&#x20;
* What kind of **interactivity** is supported (refer back to [Initial Assessment](../getting-started/initial-assessment.md))? What kind of specialised XR hardware is needed to support this?&#x20;
  * Does the experience require the use of a **controller** or other **human interface device (HID)**?&#x20;
  * If yes to above, can this be fulfilled by a generic piece of hardware or is a specific or custom-made device required?&#x20;
* Are there any technical or conceptual reasons that [**specific XR hardware**](head-mounted-display/) (e.g. [HMD](head-mounted-display/)) is needed to access the XR content?&#x20;
  * Dependency relationships with specific hardware can be baked into software when it is created (e.g. by using certain manufacturer-specific plugins).
  * A creator might prefer certain hardware for its characteristics (e.g. technical, visual, conceptual).
* **How many users** are supported simultaneously? e.g. single or multiple stations providing access, discrete or shared experience.
* Does the software require **internet access**? If so, what for and does this need to be maintained?
* Does the experience involve **sound**? How is this played back?&#x20;
  * How is **sound** played back? Is this via the HMD or is additional hardware required to support this? e.g. audio interface, speakers, headphones.
  * Is [**spatial audio**](../preserving-360-video/spatial-audio.md) utilised and if so how is it played back? e.g. via positional speakers or head-related transfer function (HRTF) through an [HMD](head-mounted-display/) or headphones.&#x20;
  * Is **subtitling or captioning** used, or might they be needed?&#x20;

## Preservation Preparedness

If specific or custom hardware is an important component of the XR material you are caring for, the following measures may help you maintain access and prepare for long-term preservation:

* Collecting multiple examples of **exemplar hardware** as a means of providing access in the short-term, particularly if access requirements are immediate.
* Create **disk images** of the internal storage media of any computers, to ensure that the complete software environment is stored independently and can be recovered in the event of hardware failure.
  * Extract and **archive any related software components** (e.g. the [XR runtime](head-mounted-display/archiving-an-xr-runtime.md) which is required to drive the XR hardware system) from the hardware.
* **Gathering documentation** of the hardware and its components.
  * For off-the-shelf hardware this will typically be very limited, as they are proprietary devices for which detailed technical specifications are not public.
  * For custom hardware devices, source or create circuit diagrams and a bill of materials to support maintenance and repair.

[^1]: **G**raphics **P**rocessing **U**nit, also known as a graphics card or video card.

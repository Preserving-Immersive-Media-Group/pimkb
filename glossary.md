# ⁉ Glossary

This glossary is an effort to define frequently encountered immersive media terminology and support a common vocabulary in collaboration between disciplines. The [first version](https://notepad.rhizome.org/ipres2019-vr-glossary) was compiled during iPRES 2019 by participants in the VR Hackathon event. Definitions are sourced from the following existing online glossaries:&#x20;

* Unity: [What is XR Glossary](https://unity.com/how-to/what-is-xr-glossary)
* [The VR Glossary](http://www.vrglossary.org/)
* XinReality wiki: [Terms](https://xinreality.com/wiki/Category:Terms)
* Oculus Creators Portal: [VR Glossary](https://creator.oculus.com/learn/vr-glossary/)
* Interactive Advertising Bureau (IAB): AR and VR Terminology [PDF](https://www.iab.com/wp-content/uploads/2018/07/IAB\_VR-AR\_Glossary\_v5b.pdf)
* [A complete Virtual Reality glossary](https://web.archive.org/web/20210123134856/https://kei-studios.com/complete-virtual-reality-glossary/)
* [VR Glossary](https://web.archive.org/web/20190516221157/https://www.ebu.ch/files/live/sites/ebu/files/Projects/VR/VR%20Glossary.pdf)
* Digital Preservation Handbook: [Glossary](https://www.dpconline.org/handbook/glossary)

To do:&#x20;

* Review and agreement on these definitions&#x20;
* Add visual examples/images to illustrate what is being described
* Add relevant digital preservation terms

## VR General <a href="#vr-general" id="vr-general"></a>

**Virtual Reality**: Virtual reality, commonly abbreviated to VR, is a technology that simulates a fully immersive virtual or imaginary environment in which a user feels that they are physically present.

**Augmented Reality**: Augmented reality, commonly abbreviated to AR, is a technology that overlays virtual elements on top of a real-world environment.

**Augmented Virtuality**: Similar to augmented reality, this refers to a technology system whereby a largely virtual environment is merged with real-life objects.

**Mixed Reality:** Described variously as either mixed reality, MR or hybrid reality, this term refers to any technology that isn’t a fully immersive VR system, but instead augmented reality or augmented virtuality (see above definitions). This is also (confusingly) used to describe Microsoft’s virtual platform, which includes both VR and AR devices.

**Three degrees of freedom**: Often abbreviated to 3DoF, this term refers to the ability to move in six directions, namely pitch, yaw and roll.

**Six degrees of freedom**: Often abbreviated to 6DoF, this term refers to the ability to move in six directions, namely pitch, yaw, roll, elevation, strafing and surging.

[**CAVE**](https://www.ebu.ch/files/live/sites/ebu/files/Projects/VR/VR%20Glossary.pdf) **(cave automatic virtual environment)**: is a virtual reality environment consisting of 3 to 6 walls that form a room-sized cube.

**On-rails**: A VR experience in which there is no significant use of positional tracking. It has a start and an end like a video.

**Scene behaviours**: Can you manipulate objects and with what interaction?

**Caching**: a grid/cache appears if you move out of the safe area.

**VR-runtime**: integration of software and hardware (specific headset drivers etc.) for VR

**Presence/immersion**: Both presence and immersion are used interchangeably to describe the sensation of feeling physically present within a virtual experience, as opposed to the detachment experienced through experiencing content via a conventional screen-based medium.

## Performance <a href="#performance" id="performance"></a>

**Frames per second**: Also known as Frame rate or fps, this measures how often images (also called ‘frames’) are shown consecutively. This is related to, yet distinct from, refresh rate (see below). 60 frames per second is usually considered playable without causing motion sickness, but the best VR headsets have even higher refresh rates.

**Refresh rate**: This specifically indicates how often the buffer is updated and an image (often called a ‘frame’) regenerated on a screen, an important element when creating a realistic virtual environment. This is measured in Hertz (Hz) and is related to, yet distinct from, frames per second (see below). A low refresh rate can cause judder (see below).

**Judder**: Typically caused by a low refresh rate (see above) or dropped frames, judder is the manifestation of motion blur (also known as smearing) and the perception of more than one image simultaneously (known as strobing). This can cause simulator sickness (see below).

[**Latency**](https://www.ebu.ch/files/live/sites/ebu/files/Projects/VR/VR%20Glossary.pdf): The time delaying virtual reality; a glitch in the VR system, when the images are not well synchronized with the sound, changing later than expected.

## Behaviour <a href="#behaviour" id="behaviour"></a>

**Teleportation**: A common method of virtual navigation, this allows the user to quickly move between points without having to traverse the distance between them.

## Rendering <a href="#rendering" id="rendering"></a>

**3D API**: A library and interface supporting common 3D rendering tasks. Examples include DirectX (Windows), OpenGL (cross-platform), Metal (MacOS), Vulkan (cross-platform).

**Ambient occlusion**: Ambient occlusion is a technique to produce film-like lighting quality with real-time performance. Ambient occlusion is a lighting model that calculates the brightness of a pixel in relation to nearby objects in the scene.

**Anti-aliasing**: Raster images are made of rectangular pixels, which can lead to jagged edges in curved lines. Anti-Aliasing aims to reduce the jaggedness created by these pixels, and there are multiple techniques to achieve this.

[**Fast Approximate Anti-Aliasing**](https://www.gamingscan.com/what-is-anti-aliasing/)**:** The least demanding type of anti-aliasing. Rather than running complex calculation depending on the geometry and colors displayed, FXAA simply applies extensive blurring to obscure the jagged edges. The end result is unnoticeable performance impact but a generally blurrier image.

[**Multi-sampling Anti-Aliasing**](https://www.gamingscan.com/what-is-anti-aliasing/): It relies on color manipulation around geometric shapes to produce an effect of smoothness. It can use either 2, 4 or 8 samples – the higher the sample count, the higher the quality and the performance impact.

[**Super Sampling Anti-Aliasing**](https://www.gamingscan.com/what-is-anti-aliasing/): What it does is make the GPU render a game at a higher resolution and then downsamples it. That way, it increases the overall pixel density of your display and renders a much sharper image.

**Bloom**: Creates blurry feathered edges to light sources in post-processing

[**Foveated rendering**](https://kei-studios.com/complete-virtual-reality-glossary/): A tracking-based rendering method where the user’s eye movements are tracked, allowing peripheral vision to be rendered at a lower quality, thus reducing the amount of processing needed to render a VR experience in real-time.

**Lens Flare**: The image is processed to replicate light reflecting in a simulated camera lens.

**Material shaders**: (PBR vs traditional methods, BSDF/BRDF)

**Shader**: A shader is a small computer program designed to run on the GPU. Shaders are written in languages associated with 3D APIs, such as HLSL (DirectX), GLSL (OpenGL) and SPIR-V (Vulkan).

**Asynchronous Reprojection / Spacewarp / Timewarp:**&#x20;

**Lens Distortion:**&#x20;

## Navigation & Tracking <a href="#navigation-amp-tracking" id="navigation-amp-tracking"></a>

[**Inside-out tracking**](https://www.vrfocus.com/2018/07/a-glossary-of-immersive-tech-terms/): the headset has all the tracking tech built-in. Disadvantage: it cannot track the controllers behind the person

[**Inside-out tracking**](https://kei-studios.com/complete-virtual-reality-glossary/): This tracking method uses cameras fixed to the device being tracked in order to determine how its position changes relative to its environment.

[**Outside-in tracking**](https://www.vrfocus.com/2018/07/a-glossary-of-immersive-tech-terms/): sensors/cameras being mounted around the user creating a tracked play space. The benefit of this design is that players are monitored wherever they go within that area, and so are the controllers.

[**Outside-in tracking**](https://kei-studios.com/complete-virtual-reality-glossary/): This term refers to the use of externally placed positional sensors to track a user moving in real-time.

[**Eye tracking**](https://kei-studios.com/complete-virtual-reality-glossary/): The measurement of eye positioning and movement to discern where exactly a user is looking. This is a crucial element of foveated rendering (see above).

**Head tracking**: This is a method of tracking a user in virtual reality whereby the picture shifts as they move or angle their head.

**Motion tracking**: The use of positional sensors and markers that register where a device is, allowing it to be mapped to a virtual environment.

[**Rotational tracking**](https://xinreality.com/wiki/Rotational\_tracking): is a term used to describe how a piece of hardware determines how tilted something is. There are three different ways that an object can rotate, we call each of these ways a degrees of freedom, and you can track any number of degrees of freedom (see above for 3DoF and 6DoF).

**Positional sensor**: Devices used to track the exact position of the user while they are using a VR system, and feedback data that is used to inform the information being shown on the screen.

**Room-scale**: A virtual reality set-up that, thanks to an expansive configuration of positional sensors (see above), allows the user to physically roam around an entire room without experiencing limitations.

**Fixed viewpoints**: Common to many VR experiences – particularly those that are mobile-based – this feature limits the user to a pre-defined number of explorable positions within a virtual reality build, rather than allowing open-world exploration.

**First or Third person Experience**: Whether the user experiences the virtual world as through their own eyes, or as an external observer.

## Side Effects <a href="#side-effects" id="side-effects"></a>

**VR sickness**: typically involves symptoms of dizziness and nausea.

**Simulator sickness**: Sometimes referred to as VR sickness and with similar effects to motion sickness, this can be caused by factors including judder and users perceiving self-motion when stationary.

[**Asynchronous timewarp**:](https://www.newegg.com/vr/guides/vr-terms-you-should-know.html) a middle-ground between high persistence and low persistence displays that “warps” a current frame to compensate for the motion of your head before showing you the next rendered frame.

**Spatial desync**: the effect or difference occurring when a user’s movements in real life and the VR avatar’s movements are out of sync.

## Peripherals <a href="#peripherals" id="peripherals"></a>

### Head Mounted Displays (HMD) <a href="#head-mounted-displays-hmd" id="head-mounted-displays-hmd"></a>

**Computer-based or tethered HMD**: describes any headset that requires a connection to a stand-alone PC in order to function. Well-known computer-based systems include Facebook’s Oculus Rift and the HTC Vive.

**Mobile-based HMD**: Any HMD where the processing and display for the VR experience are provided by a mobile phone. Notable examples include the Samsung Gear VR and Google Daydream headset.

**Standalone HMD**: A VR or AR HMD where the entire system is self-contained within the device. Examples include the Microsoft HoloLens mixed reality headset and the upcoming Oculus Go from Facebook.

### Sound <a href="#sound" id="sound"></a>

Headphones are usually provided with or within HMD’s. Specifications are often contingent to brand but common features may include 3D spatial sound for an immersive experience.

**Binaural**:&#x20;

### Hand controllers <a href="#hand-controllers" id="hand-controllers"></a>

Peripheral device/s, often left and right to provide full motion tracking of a player’s hands in VR experience/play.

## Preservation

### General

**Complex Digital Objects:** An object, item, or work with a component that is digital, is made up of multiple files (likely of differing file formats) and may or may not incorporate a physical component. A Complex Digital Object is likely to depend on software, hardware, peripherals, and/or networked or non-networked data, platforms, and/or services. Contrast with a **Simple Digital Object** which consists of a single file. XR materials can be considered Complex Digital Objects.&#x20;

### Documentation

### Emulation

### Migration

### Code Migration




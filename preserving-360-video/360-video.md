# Introduction

**360-degree video** is a form of moving image sequence that surrounds the viewer in virtual space. When wearing an [HMD](../preserving-xr-hardware/head-mounted-display/#head-mounted-displays), the viewer is able to freely rotate their head, determining their viewing direction. This can be contrasted with traditional, fixed-perspective video in which the viewing angle is fixed.

As the video content is linear, the viewing position is either fixed or follows a pre-determined path ("on rails") captured in the video. However, a degree of positional interactivity can be introduced through hotspots or portals which, when interacted with in the virtual scene, jump the viewer to another piece of 360-degree video content. Adding these requires the use of a software layer in addition to the video, which places the content somehwere between 360-degree video and [3D software](/broken/pages/9dvten2QyRPU1DJQKfXD).

360-degree video can be created in a number of different ways:

* Captured by a **camera** or array of camera lenses;
* Generated as an export from **3D rendering software** (e.g. Blender);
* Generated from a **real-time 3D** [**game engine**](../preserving-3d-software/game-engines/#list-of-engines) (either as a standalone experience or as documentation of a real-time 3D VR experience).

It is then played back using video playback software that supports 360° video and viewed via [XR hardware](../preserving-xr-hardware/head-mounted-display/).&#x20;

## Assessing 360-degree Video

* How was the 360-degree video **created**?&#x20;
  * Was it created through **camera capture**?&#x20;
    * If so, is the camera model and captured video format known?
  * Was it created using a **3D software tool** e.g. 3D renderer or game engine?&#x20;
    * Is the capture and output format of the video known?&#x20;
  * Did the video undergo a **stitching** process
    * Is the software used for stitching known?&#x20;
  * Was the video **edited**?&#x20;
    * If so, what software was used?&#x20;
    * Are these production assets available?&#x20;
* By inspecting file **metadata**, are you able to determine key characteristics of the 360-degree video format? If not you will need to determine these manually. See [Video Formats](video-formats.md) for more information about these.
  * The [projection format](video-formats.md#projection-format) used e.g. cubemap, equirectangular.&#x20;
  * Whether the video is [monoscopic or stereoscopic](video-formats.md#monoscopic-vs-stereoscopic).
  * The [codec and pixel format](video-formats.md#video-file-format) that the video has been encoded with.
* What kind of **audio format** does the video use?&#x20;
  * If this uses [spatial audio](spatial-audio.md), how was this created?&#x20;
  * How has the spatial audio been encoded in the video file?&#x20;

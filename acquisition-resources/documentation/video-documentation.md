# Video Documentation

Video documentation can be used to record aspects of an immersive media (IM) experience. This can take two forms:&#x20;

* Physical capture: Video recording of the real-world physical actions of a user interacting with an IM experience.&#x20;
* Virtual capture: Video recording of the virtual actions of a user interacting with an IM experience, as would be sent to a display device.&#x20;

## Virtual Video Capture

Virtual video capture can produce two kinds of video:

* **Fixed-perspective video**: video which representing a fixed perspective on the virtual environment; the standard form of video designed for non-interactive viewing.
* [**360 video**](../../understanding-immersive-media/360-video/): video representing a 360 degree view from a central point, therefore allowing a level of interactivity via rotational tracking.

### Capturing Video from an Application

Hardware and software tools can be used to capture video from a real-time 3D application. This can be fixed-perspective or 360 video.&#x20;

#### Software Tools

| Tool                                                                                                                                               | Description                                                                                   | Capture Formats |
| -------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- | --------------- |
| [Open Broadcaster Software (OBS)](https://obsproject.com/)                                                                                         | Free and open source software for video recording. Cross-platform (Windows, MacOS and Linux). |                 |
| [NVIDIA ShadowPlay](https://www.nvidia.com/en-gb/geforce/geforce-experience/shadowplay/)                                                           | Requires NVIDIA GPU.                                                                          |                 |
| [Xbox Game Bar](https://support.microsoft.com/en-us/windows/record-a-game-clip-on-your-pc-with-xbox-game-bar-2f477001-54d4-1276-9144-b0416a307f3c) | Windows 10/11 built-in tool.                                                                  |                 |

### Rendering Fixed-Perspective Video in the UE4 Editor

{% hint style="info" %}
Tested in version 4.27 of the editor only.
{% endhint %}

The Unreal Engine 4 editor has built-in tools which allow export of video sequences. The actions of these sequences can be scripted or recorded from user interaction within the editor. Using them therefore requires access to the source project and a level of engagement with the editor software. This will may involve modification of the source project, so you may wish to work with a copy or version control system.&#x20;

#### Render Formats and Settings

Video export format depends on the options you select in the Render Movie Settings dialogue (info derived from MediaInfo output applied to rendered video):&#x20;

* With 'Use Compression' unchecked: RGBA (8 bits-per-channel) in AVI with OpenDML extension container.
* With 'Use Compression checked: MJPG video (YUV, 4:2:2, 8 bits-per-channel), Interlaced, Top Field First) in AVI container.

![The Render Movie Setting Dialogue in Unreal Engine 4.27.](../../.gitbook/assets/UE4\_4\_27\_RenderMovieSettings.png)

There are some configurable options, including output video resolution and framerate.&#x20;

The uncompressed video option yields the best quality output but the video files produced are VERY large - in our test 8 sec of capture (1080p at 24fps) yielded a 1.5 GB file. Take care that you have enough storage space to capture in this format if you are going to use this setting, at which point you can convert to lossless compression format like FFV1 for storage.&#x20;

#### Workflow

In order to generate a video from a UE4 project using the editor tools, you need to first create a _sequence_: a scripted or recorded set of events occurring within the virtual environment. Some projects may already use a sequence to choreograph the actions that occur within the IM experience (e.g. an 'on-rails' experience). In these cases, locate the sequence in the Content Browser and open it. In the toolbar you should see a clapperboard icon, which will open up the Render Movie Settings dialogue.&#x20;

![](../../.gitbook/assets/UE4\_4\_27\_Sequencer\_Render.png)

Where there is not an existing sequence, you can create a sequence by scripting or [recording](https://docs.unrealengine.com/4.27/en-US/AnimatingObjects/Sequencer/Overview/TRReferenceGuide/) interaction in the engine.&#x20;

### Rendering 360 Video in the UE4 Editor

360 video can be created with a workflow that utilizes plugins enabling export of stereoscopic frames from UE4, which are then assembled into a video sequence with software like Adobe After Effects (which has support for VR and 360 video).

The following workflow uses [Panoramic Capture Tool](https://docs.unrealengine.com/4.27/en-US/WorkingWithMedia/CapturingMedia/StereoPanoramicCapture/), a free plugin included with UE4.

Note that there are some caveats to using Panoramic Capture Tool:

* It does not export audio.
  * Audio could theoretically be pulled from fixed-perspective video of an "on-rails" experience, but another strategy would be required for interactive content.
* It is an Experimental feature in UE4, and is not as actively developed or supported as other UE features.
* UE v4.19 and earlier use a different version of Panoramic Capture that does not have the benefit of Blueprints, and requires some manual programming; this earlier version is not covered here.

There are other 360 export tools that can be purchased in the Unreal marketplace.

#### UE4 Panoramic Capture Tool Workflow

\[workflow to be added here]

## Physical Video Capture

\[To be added]

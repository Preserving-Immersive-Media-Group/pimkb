# Spatial Metadata

Due to the additional properties of 360-degree video in comparison to fixed-perspective video, there is a need for metadata standards to accommodate this. These are an important component of documentation for 360-degree video files as they support correct identification and decoding by playback tools. Google has released a suite of standards and metadata injection tools on GitHub under the name [Spatial Media](https://github.com/google/spatial-media).

In order to have 360-degree video recognised (e.g. when using a video player, or uploading to YouTube) and played back properly, spatial metadata must be included in the file-level metadata. [Spatial Media Metadata Injector](https://github.com/google/spatial-media/releases/tag/v2.1) is open source software, developed by Google, that can be used to inject spatial metadata into 360-degree video files. This supports MOV, MP4 and MKV/WebM (video only) containers.&#x20;

It supports adding metadata describing:

* Projection type
* Stereoscopic mode
* Projection pose (yaw, pitch, roll) - presumably for initiation position?&#x20;
* Spatial audio including ambisonic channel order and mapping

You can find full specification information on GitHub for the supported elements describing [video](https://github.com/google/spatial-media/blob/master/docs/spherical-video-v2-rfc.md) and [audio](https://github.com/google/spatial-media/blob/master/docs/spatial-audio-rfc.md).&#x20;


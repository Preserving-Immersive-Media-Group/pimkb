# Metadata Standards

Due to the increased complexity and number of variables in 360 video, there is a need for metadata standards to accommodate this. Google has a suite of standards and metadata injection tools on GitHub under the title of "spatial media" [here](https://github.com/google/spatial-media).&#x20;

In order to upload 360 video to YouTube and have it recognised and played back properly, it is [required](https://support.google.com/youtube/answer/6178631) that spatial metadata be injected using the Google tool. This supports MP4 and WebM (video only) containers. You can find specification information on GitHub for the support elements for [video](https://github.com/google/spatial-media/blob/master/docs/spherical-video-v2-rfc.md) and [audio](https://github.com/google/spatial-media/blob/master/docs/spatial-audio-rfc.md).&#x20;

It supports:

* Projection type
* Stereoscopic mode
* Projection pose (yaw, pitch, roll) - presumably for initiation position?&#x20;
* \[Add audio]

### Spatial Media Metadata Injector

[Spatial Media Metadata Injector](https://github.com/google/spatial-media/releases/tag/v2.1) is a open source software that can be used to "convert standard" videos (equirectangular for example) to inject 360° / stereoscopic 3D (top/bottom) and spatial audio (ambix / sn3df) datas




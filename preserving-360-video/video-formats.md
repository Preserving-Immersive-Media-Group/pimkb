# Video Formats

## 360-degree Video Format Properties

360-degree video formats build on those used for fixed-perspective video, and the container and codec formats will be familiar to those who have worked with digital video in the past. Additional characteristics, used to support playback at 360-degrees, and common formats are described below.&#x20;

### Monoscopic vs Stereoscopic

360-degree video can be either monoscopic or stereoscopic:

* **Monoscopic** 360-degree video contains video captured from a single viewpoint and supports what is perceived as a 2D representation of the scene (i.e. there is no perception of depth).&#x20;
* **Stereoscopic** 360-degree video supports a 3D representation of the scene (i.e. there is depth perception) by capturing two different viewpoints, one for each eye. These are typically packed into a single video file, where they can be arranged side-by-side or top-bottom.

### Projection Format

Projection format refers to the way in which data representing a 360-degree or spherical field-of-view is mapped to a flat image when it encoded. This is similar to the way in which a map of Earth is a flat representation of the spherical surface of the planet.&#x20;

Common projection formats include:

* Equirectangular
* Cubemap
* Equi-angular cubemap
* Pyramid

Choice of projection format has an impact on the quality of the video (pixel density may differ across the image once it is projected) and support from different video players and streaming platforms.&#x20;

### Container Format

Container formats are familiar and widely-supported formats used for many forms of digital video, such as MOV, MP4 and MKV/WebM (WebM is based on the Matroska spec). These are also the formats which support [spatial metadata](spatial-metadata.md).&#x20;

### Video Codec

Generally, lossy, high efficiency and low-bitrate codecs are favoured for 360-degree video due to the demanding playback requirements posed by the high resolution frames. Common codecs include h.264/AVC, h.265/HEVC, VP9 and AV1. It may be possible to request that a higher quality format, be it playable on contemporary hardware or not,&#x20;

### Audio Codec



## Transcoding

To correctly manage 360-degree video properties such as projection format and stereoscopy while transcoding, a tool which supports 360-degree formats should be used. The [ffmpeg filter v360](https://ffmpeg.org/ffmpeg-filters.html#v360) allows conversion between 360-degree formats. &#x20;


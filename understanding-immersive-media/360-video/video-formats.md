# Video Formats

### Monoscopic vs Stereoscopic

360° video can be either monoscopic or stereoscopic. Monoscopic video supports what is perceived as a 2D representation of the scene i.e. there is no perception of depth. Stereoscopic video supports a 3D representation of the scene with a perception of depth.&#x20;

* **Monoscopic** 360° video contains video captured from a single viewpoint within the scene.
* **Stereoscopic** 360° video contains video captured from two viewpoints within the scene. These viewpoints can be different point of view for each eye. These are packed into a single video file where they can be arranged side-by-side or top-bottom.

### Video File Format

Codecs: h.264/AVC, h.265/HEVC, VP9

Wrappers: MP4, Mastroska, WebM

Significant variables in choice of video file format:

* Achievable bitrate / compression
* Metadata container options
* ...?

### Projection Format

Projection format refers to the way in which data representing a 360° or spherical field of view is mapped to a flat image when it encoded. It is similar to the way in which a map of Earth is a flat representation of the spherical surface of the planet.&#x20;

Some common projection formats include:

* Equirectangular
* Cubemap
* Equi-angular cubemap
* Pyramid

Significant variables in choice of projection format:

* Pixel density
* Tool support (encoding, decoding)
* Requirements of video streaming platforms (e.g. YouTube)
* ...?


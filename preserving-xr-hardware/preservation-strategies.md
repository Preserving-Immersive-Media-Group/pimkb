# Preservation Strategies

Computer hardware is difficult to preserve in the very long-term as its maintenance is dependent on access to suitable components and specialist knowledge, both of which can be lost with time. XR hardware provides a particularly challenging case study given its complexity and the proprietary nature of most of the equipment available. However, there is the possibility to maintain and repair in the near term, and, providing the appropriate preparations are made, migrate to different hardware should this become unsustainable. Thinking within museum timescales however, hardware-centric preservation is unlikely to be sustainable in the very long-term.

## Maintenance and Repair

Extending the service life of hardware through repair could support preservation efforts if a particular XR system is required. These hardware systems are meant to be used, and in an exhibition context they can be subjected to serious wear and tear.

The consumer market for XR hardware systems and mobile phones is built on planned obsolescence; products are superseded by new models, manufacturers only provide limited warranty periods for repair or replacement, and parts are not commonly available. Purchasing backup equipment or sourcing equipment to be used for parts may be a sensible part of a preservation plan. Valve have bucked the trend by making available a complete set of spares for their Index HMD though iFixit. For this reason, the Valve Index is our current recommendation for a sustainable, tethered headset.&#x20;

iFixit is a US-based company that advocates for reparability of consumer devices. The Preserving Immersive Media Group has no affiliation with iFixit. The guides linked in the table below provide step-by-step instructions, with photos, recommended tools and in a few cases the option to purchase replacement parts. Their teardown reviews are another resource should you have equipment that is intended to be used for parts. Popular XR systems and Samsung Gear VR are linked here, but many other device guides can be found on iFixit.

| Hardware Model         | Repair Guide(s)                                                                                            | Source for Spares\*                                                                                         |
| ---------------------- | ---------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- |
| **Valve Index**        | [https://www.ifixit.com/Device/Valve\_Index](https://www.ifixit.com/Device/Valve_Index)                    | [https://www.ifixit.com/en-gb/Parts/Valve\_Index](https://www.ifixit.com/en-gb/Parts/Valve_Index)           |
| **Meta Quest Devices** | [https://www.ifixit.com/Search?query=meta+quest](https://www.ifixit.com/Search?query=meta+quest)           | [https://www.fixmyoculus.com/](https://www.fixmyoculus.com/) (USA)                                          |
| **Oculus Devices**     | [https://www.ifixit.com/Search?query=oculus](https://www.ifixit.com/Search?query=oculus)                   | [https://www.fixmyoculus.com/](https://www.fixmyoculus.com/) (USA)                                          |
| **HTC Devices**        | [https://www.ifixit.com/Device/HTC](https://www.ifixit.com/Device/HTC)                                     | [https://www.ifixit.com/en-gb/Parts/HTC\_Vive](https://www.ifixit.com/en-gb/Parts/HTC_Vive) (limited range) |
| **Samsung Gear VR**    | [https://www.ifixit.com/Search?query=samsung+gear+vr](https://www.ifixit.com/Search?query=samsung+gear+vr) |                                                                                                             |

\*Valve are the only manufacturer supplying official spares for all parts of their hardware. Aftermarket options (e.g. salvage from failed devices) may be best option for anything else.

## Hardware Migration

If maintenance becomes impossible, we can instead look to migrating to new hardware — a process known as hardware migration. In the early history of the 'second wave' of XR hardware, a lack of standardisation and poor compatibility between hardware and software meant that this was unlikely to be successful — or at least require a degree of modification to the software before I would be successful. However, with the widespread adoption of the [OpenXR standard](head-mounted-display/openxr.md), this becomes a realistic possibility.&#x20;

That said, there are likely to impacts to a change in XR hardware, even where compatibility is no issue. This is simply a result of variation in the hardware properties (e.g. the&#x20;lower resolution panels and restricted field-of-view found in earlier models) that can form a distinctive character, which may or may not be significant to the actual preservation of that particular XR experience.&#x20;

Nonetheless, there is no doubt that ensuring OpenXR support is built into any XR application is the best possible to way to support future hardware migration. With the release of OpenXR 1.0, the maintainers of OpenXR, the Khronos Group, [stated that](https://www.khronos.org/news/press/khronos-releases-openxr-1.0-specification-establishing-a-foundation-for-the-ar-and-vr-ecosystem) they would continue to develop the standard while "maintaining full backwards compatibility from this point onward". This is excellent news for preservation work and means that it should be possible to run older XR applications built with OpenXR 1.0 (or later) support on any contemporary XR hardware supporting the standard.

---
title: Major improvements to most file conversions
description: "We’ve just rolled out a massive under-the-hood update that improves the quality of many conversions, while also adding new ones."
image: major-update.webp
image_alt: Major MConverter conversion engine update
date_added: 2026-05-21
date_updated: 2026-05-27
author: martin-minchev
aside_cards:
  - 50-percent-discount-max
  - mobile-app
---

I’m excited to announce a big update to our conversion engine that’s just been released to all [PWA](https://mconverter.eu/) and [MConverter API](https://dev.mconverter.eu/) users.

Tons of bugs have been fixed and improvements have been made to pretty much all supported formats. Some noteworthy changes include:

* Creating animated JPEG XL (JXL) images is now supported. They can be converted from all video formats, animated GIF and WebP, as well as vice-versa.  
* Easily export all image [frames from animated AVIF](https://mconverter.eu/convert/avif/png/) files. You can get them as a sorted ZIP of PNGs, for example, or [as layers in a PSD](https://mconverter.eu/convert/avif/psd/) file. AVIF animations can also be [exported to pages in a PDF](https://mconverter.eu/convert/avif/pdf/).  
* You can now [convert animated WebP to animated AVIF](https://mconverter.eu/convert/webp/avif/).  
* Significantly improved the processing speed when creating AVIF animations from a video or animated GIF.  
* Image metadata (such as EXIF, date taken, GPS location, etc.) is now consistently kept by default in the converted file when converting image-to-image. This behavior allows you to easily free up space by converting your JPG images to more efficient formats, such as [WebP](https://mconverter.eu/convert/jpg/webp/), [AVIF](https://mconverter.eu/convert/jpg/avif/), and [JPEG XL](https://mconverter.eu/convert/jpg/jxl/). After doing that, you can delete the original JPG files, knowing that no image quality or metadata has been lost.  
* Properly handle and display newer emoji in documents, PDFs, and images.  
* Fixed disappearing images when converting from [Markdown to Word](https://mconverter.eu/convert/markdown/docx/) and other similar instances. Embedded images will now remain after the conversion.  
* Fixed some errors when converting images taken with Google Pixel phones, with Ultra HDR turned on.  
* Fixed a conversion error when processing iPhone photos taken with specific settings.  
* Fixed a conversion engine crash when converting a GIF or [video to AVIF](https://mconverter.eu/convert/mp4/avif/), when the source file’s width or height is less than 65 pixels.  
* Fixed an error impacting videos with a reserved color space.  
* ...and many others.

As always, each format has been tested in an automated way, but also manually by a human reviewer to ensure the most accurate results. While automations with artificial intelligence can be cool, they’re inherently prone to mistakes and hallucinations. For this reason, unlike some competitors, we have **not** reduced the importance of the human element in the process.

Nonetheless, if we’ve missed anything and you’re experiencing an issue, please [let us know](#legal) and we’ll gladly help.

![Some of the new improvements to MConverter](mconverter-improvements-bento-grid.webp)
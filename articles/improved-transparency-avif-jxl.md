---
title: Improved transparency handling for AVIF, JXL, WebM, and more
description: MConverter can now produce animated AVIF files with transparency!
image: conversion-updates.webp
image_alt: Opacity and transparency updates
date_added: 2026-10-29
date_updated: 2026-10-29
author: martin-minchev
categories:
  - updates
  - image-conversion
  - video-conversion
aside_cards:
  - 50-percent-discount-max
  - mobile-app
---

The emphasis of this MConverter update is on how transparency and opacity are handled in newer image formats.

## AVIF transparency

For a long time, MConverter could only preserve transparency in AVIF when converting from a limited number of formats, such as PNG. But that’s no longer the case!

Now, if your input file has an alpha channel or other opacity information, the AVIF file produced by MConverter will retain it. This means that you can also convert videos and [GIFs to animated AVIF](/convert/gif/avif/) images with transparency. [WebP animations with alpha](/convert/webp/avif/) can be converted to AVIF too.

## JXL (JPEG XL) transparency

[AVIF to JXL](/convert/avif/jxl/) conversions now support transparency. Conversions from other formats to JXL already handled both transparency and animations.

## Converting WebM videos with transparency

If you have a WebM video that contains transparent areas, you can now convert it to [animated WebP](/convert/webm/webp/), [AVIF](/convert/webm/avif/), or [JXL](/convert/webm/jxl/), and the transparency will be kept. Both VP8 and VP9 codecs are supported for decoding transparency data.

## Fixed WebP frame stacking glitch

When converting most [video formats to WebP](/convert/mov/webp/), transparent areas could cause a visual glitch in which each subsequent frame got stacked on top of the previous ones. This problem has been fixed, so the resulting animation should now look like your original file.

If you notice any issues with transparency handling, please [let us know](#legal) and we’ll gladly help.
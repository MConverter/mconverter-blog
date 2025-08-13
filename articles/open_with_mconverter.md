---
title: Convert right from your file manager | File Handling API
description: MConverter can now be used via the right-click menu option to “Open with…”
image: open_with_mconverter.webp
image_alt: Right-click context menu on Windows 10, showing MConverter as an option
date_added: 2023-06-01
date_updated: 2023-06-01
categories:
  - tips_and_tricks
  - technical
aside_cards:
  - app
---

You may have noticed a new app show up in the **“Open with…”** context menu of your File Explorer: MConverter. That's right, you can now queue files for converting without having to switch away from your file manager.

<iframe src="https://www.youtube-nocookie.com/embed/OP9ryr7cgR8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

This feature works when MConverter is installed via Google Chrome or Microsoft Edge on all major desktop operating systems, including Windows, macOS, Linux, and ChromeOS. The [MConverter app](https://www.microsoft.com/store/productId/9N4F69HXK2LP) from the Microsoft Store is supported as well.

## How to queue multiple files for converting?

First, select files by holding Ctrl or Shift while clicking on them. Alternatively, click and drag your cursor over them. You can also select all files in a folder with Ctrl+A. Then, drag the selected files over the MConverter icon – even if the app is not open.

## I'm a curious web developer. How was this implemented?

The MConverter progressive web app uses the File Handling API for opening our supported file types. You can learn how to implement this in your PWA here: [Let installed web applications be file handlers](https://developer.chrome.com/en/articles/file-handling/).
---
title: Texture Creation
description: Details about how to create VTF textures for use in Chaos
published: true
date: 2022-11-07T06:32:20.822Z
tags: engine, materials
editor: markdown
dateCreated: 2022-10-26T07:47:43.012Z
---

# Texture Creation

Textures may be easily created using the new vtex2 command line and GUI tool.

## GPU-friendly Compressed Image Formats

As of August 2022, Chaos Engine has native support for the following compressed texture formats:
* DXT1
* DXT5
* BC4 (named ATI1N in engine)
* BC5 (named ATI2N in engine)
* BC7 (VTF 7.6 Only)

## Auxiliary Compression (VTF 7.6 Only)

As of September 2022, Chaos Engine has support for lossles DEFLATE "auxiliary" compression to further reduce image data size. Unlike the BCn formats, DEFLATE isn't actually an image format, rather it compresses arbitrary image data in the VTF to reduce disk size. This doesn't reduce texture video memory use, as the texture is decompressed as it's loaded off the disk.

DEFLATE compression can reduce on-disk texture size by 40% on average.
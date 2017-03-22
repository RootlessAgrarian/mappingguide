# Editor backgrounds for custom modules

This tutorial teaches you how to make a custom editor background, the reference map image that appears in the editor when you press 'A'.

This part will describe how to take a map image and import it into the SCS Editor. A technique for getting high-resolution map images can be found in [part 1](1_imagery.md).

1. Image size & format

## 1. Image size & format

The editor background image needs to be a DDS format image with width and heights that are both divisible by 4. Because our image is square, we'll use the game texture convention of using square numbers. (i.e. 512, 1024, 2048, 4096)

A DDS format plugin for Adobe Photoshop can be downloaded from the [NVIDIA developer site](https://developer.nvidia.com/nvidia-texture-tools-adobe-photoshop), and for free software both [Paint.NET](http://www.getpaint.net/index.html) and the [GNU Image Manipulation Program](https://www.gimp.org/) have built-in support for DDS.

Ensure that that the exported DDS file fits the dimension requirements, and is exported as DXT5. Mipmaps are not necessary for the image.

![Paint.NET canvas size adjustment](img/2_crop.png)
![Paint.NET export settings](img/2_dds.png)

You should now have a compatible image. You can copy our version from the GitHub repo [here](#).

## 2. 
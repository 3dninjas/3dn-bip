# 3D Ninjas | Blender Image Preview (BIP) Library

## Documentation

1. [Getting Started (this page)](https://3dninjas.github.io/3dn-bip/)
2. [Install Pillow](https://3dninjas.github.io/3dn-bip/install_pillow/)
3. [Reference](https://3dninjas.github.io/3dn-bip/reference/)
4. [More](https://3dninjas.github.io/3dn-bip/more/)
5. [Development](https://3dninjas.github.io/3dn-bip/development/)

## What is 3DN BIP?
*3DN BIP* or *3D Ninjas Blender Image Preview* is a library, which allows blazingly fast preview image loads in Blender. Furthermore, it can load preview images of arbitrary size. It operates as an `bpy.utils.previews` drop-in replacement and does all the heavy lifting for you.

Our library enables the following major use cases:

1. Load preview images shipped as BIP images blazingly fast. We recommend this approach in case you can generate the images beforehand. In this case, your users don't need to take any action to enjoy the speed boost.
2. Load regular JPEG or PNG preview images blazingly fast. Recommended in case you need to load images provided by the user or by external software tools. For that, we need [Pillow](https://pypi.org/project/Pillow/) on the user's system. It would be best if you use our prepared `InstallPillow` operator so that your users can enjoy the speed boost with a simple click.

Notes:

1. Our library will always fall back to `bpy.utils.previews` if unsupported formats are to be loaded. For this reason, there is absolutely no disadvantage in using this library. In the worst case, we will apply the standard mechanism of Blender.
2. `.bip` is a highly optimized image format, which can be transferred to Blender's internal data structures immediately. It is always blazingly fast, whether [Pillow](https://pypi.org/project/Pillow/) is installed or not.

## Examples

Download the following sample addons. You can easily install the ZIP files in Blender via the addon preferences tab.

- Getting Started: [t3dn_bip_getting_started.zip](https://github.com/3dninjas/3dn-bip/releases/latest/download/t3dn_bip_getting_started.zip)
- Showcase: [t3dn_bip_showcase.zip](https://github.com/3dninjas/3dn-bip/releases/latest/download/t3dn_bip_showcase.zip)

## Library

The latest release of the library can be downloaded here: [t3dn_bip.zip](https://github.com/3dninjas/3dn-bip/releases/latest/download/t3dn_bip.zip)

Just extract the zip file and copy the folder into your addon. Take a closer look at the examples given above to learn how to use the library.

In case you want to install the library via [PyPI](https://pypi.org/project/t3dn-bip/), you can use the following command:

```sh
python -m pip install t3dn-bip
```

## Converter

The converter is provided via [PyPI](https://pypi.org/project/t3dn-bip-converter/). Use the following command for the installation:

```sh
python -m pip install t3dn-bip-converter
```

Use the following command to convert images of [various formats](https://pillow.readthedocs.io/en/stable/handbook/image-file-formats.html) into the BIP format:

```sh
python -m t3dn_bip_converter source_file.png destination_file.bip
```

## Showcases

### Show `.bip` and `.jpg` Images in a Panel

<a href="https://www.youtube.com/watch?v=WUcGWo9gad4&list=PLzkRr8BNKzgHKSkpBgRgCbDZlEjYypz-5"><img src="https://img.youtube.com/vi/WUcGWo9gad4/maxresdefault.jpg"></a>

### Show `.bip` and `.jpg` Images in an Enum

<a href="https://www.youtube.com/watch?v=H9-hCtpOLoo&list=PLzkRr8BNKzgHKSkpBgRgCbDZlEjYypz-5"><img src="https://img.youtube.com/vi/H9-hCtpOLoo/maxresdefault.jpg"></a>

### Show large `.bip` and `.jpg` Hero Images in a Panel

<a href="https://www.youtube.com/watch?v=W_xV93_M1Ak&list=PLzkRr8BNKzgHKSkpBgRgCbDZlEjYypz-5"><img src="https://img.youtube.com/vi/W_xV93_M1Ak/maxresdefault.jpg"></a>

### Show `.bip` and `.png` Images with an Alpha Channel

<a href="https://www.youtube.com/watch?v=60D5l18AYy0&list=PLzkRr8BNKzgHKSkpBgRgCbDZlEjYypz-5"><img src="https://img.youtube.com/vi/60D5l18AYy0/maxresdefault.jpg"></a>
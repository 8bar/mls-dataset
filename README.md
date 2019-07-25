# Multiple Light Source Dataset for Colour Research (work in progress)

+ Images of **24 multiple object scenes**.
+ Each scene is taken under **18 multiple light source illumination scenarios**, the illuminants are varying in dominant spectral colours, intensity and distance from the scene.
+ **Spectral characteristics** of the camera, illuminants sources and uniformly coloured object surfaces.
+ Pixel-by-pixel ground truth annotation of uniformly coloured object surfaces.

We mainly address the realistic scenarios for evaluation of computational colour constancy algorithms, but also have aimed to make the data as general as possible for computational colour science and computer vision. 
<!--Details have been published in: [Multiple Light Source Dataset for Colour Research ](hhtp://) -->

<!--If you use this dataset, please, cite the appropriate paper.

    @article{smagina2019multiple,
    title={Multiple Light Source Dataset for Colour Research},
    author={Smagina, Anna and Grigoryev, Anton and Ershov, Egor},
    journal={arXiv preprint arXiv:},
    year={2019}
    } -->

## Image data

![Scenes overview](./images/scenes_overview.png) 

An overview of all 24 recorded MLS scenes is given on the figure above.

Each scene was constructed inside a 60x60x60 cm softbox and illuminated from the outside.
Illumination of each scene is varied in 18 configurations:

![Lighting overview](./images/lighting_overview.png) 

Each image of the scene is marked with a list of the turned-on light sources, which are ones of the following:

+ 2HAL are two halogen lights, installed at the distance about 1.2 m each; form the lighting close to embient, 
+ DESK is a desktop lamp installed at 20 cm from the softbox, 
+ R025, R050, RG025, BG025 etc is a 3-colored (red, green, blue) LED strip mounted at the top of softbox; the letters R, RG, GB or B indicates turned-on colored components of the LED-lapm, while the numbers 025, 050, 070 and 100 indicates the percentage of the emitting power.

The shooting was performed with the white balance adjusted to 6500K. 
No additional white balance correction was performed during the post-processing of the images.

**Full resolution (2391 x 1900)**

[32-bit tif images](http://vis.iitp.ru/mls-dataset/images_32bit.zip) 15 GB

[masks](http://vis.iitp.ru/mls-dataset/masks_32bit.zip) 3 MB

**Half-resolution (1280 x 1051)**

[16-bit lossless compressed png images](http://vis.iitp.ru/mls-dataset/images_16bit.zip) 2.6 GB

[masks](http://vis.iitp.ru/mls-dataset/masks_16bit.zip) < 1 MB

**Quarter resolution (600 x 493) for preview**

[jpeg images](http://vis.iitp.ru/mls-dataset/images_preview.zip) 160 MB

[masks](http://vis.iitp.ru/mls-dataset/masks_preview.zip) < 1MB

<!-- 
Images files are organized as follwoing:

<pre>
├── 01
│   ├── 01_2HAL_DESK_B025.tif
│   ├── 01_2HAL_DESK_B050.tif
│   ├── 01_2HAL_DESK_B075.tif
│   ├── 01_2HAL_DESK_B100.tif
│   ├── ...
│   ├── 01_2HAL_DESK.tif
│   └── 01_2HAL.tif
├── 02
│   ...
├── 03
│   ...
</pre>

where 01, 02, 03 etc directories containes images for a single scene, and 2HAL, 2HAL_DESK, 2HAL_DESK_B025 indicates various lighting conditions of a given scene. The scene is provided with one mask ([scene_number].png). -->

<!-- ## Spectral data

[camera]() MB
[illuminants]() MB
[surfaces]() MB

**Camera**

**Illuminants**

**Surfaces** -->

## License & citation  

Copyright 2018 Visillect Service LLC
Developed for Kharkevich Institute for Information Transmission Problems of the Russian Academy of Sciences (IITP RAS)

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />Licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>

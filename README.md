[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FElectricRCAircraftGuy%2FeRCaGuy_3D_Parts&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=views+%28today+%2F+total%29&edge_flat=false)](https://hits.seeyoufarm.com)

[>> Sponsor Me on GitHub <<](https://github.com/sponsors/ElectricRCAircraftGuy)

# eRCaGuy_3D_Parts

CAD parts, STL files, etc., to be printed by a 3D printer.

By Gabriel Staples


# Table of Contents
<details>
<summary><b>(click to expand)</b></summary>
<!-- MarkdownTOC -->

1. [License](#license)
1. [Models](#models)
1. [Notes](#notes)
    1. [3D Lithophanes \(3D-printed transparency images\)](#3d-lithophanes-3d-printed-transparency-images)

<!-- /MarkdownTOC -->
</details>


<a id="license"></a>
# License
All of my content in this repo, including my content linked-to from here but stored on other sites, such as on www.TinkerCad.com, is licensed under **[CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/) (Creative Commons Attribution-ShareAlike 4.0 International)** unless stated otherwise.

This is a copy-left license, meaning that "if you remix, transform, or build upon the material, you must distribute your contributions under the same license as the original." This license _does_ allow for commercial use. Since it is copy-left and *does* allow for commercial use, it is comparable to the GPL license if you're familiar with that license in software. 

If you are benefiting from my creations, it would mean a lot to me if you would [Sponsor Me on GitHub](https://github.com/sponsors/ElectricRCAircraftGuy). If you are a company benefiting from my creations, please choose an amount appropriate to the value you're receiving.

If this repo ever gets to the point you'd like to buy a [CC BY 4.0 license](https://creativecommons.org/licenses/by/4.0/) or other type of license instead, so that you do _not_ have to share and release your modifications under the same CC BY-SA 4.0 copyleft open source license, reach out to me and we can work out a one-time payment or [GitHub sponsorship](https://github.com/sponsors/ElectricRCAircraftGuy) in exchange for a license better suited to meet your need.

Regardless, I hope you find this useful.


<a id="models"></a>
# Models

1. todo

<iframe width="725" height="453" src="https://www.tinkercad.com/embed/hrsKxOk1Xc7?editbtn=1" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"></iframe>


<a id="notes"></a>
# Notes

<a id="3d-lithophanes-3d-printed-transparency-images"></a>
## 3D Lithophanes (3D-printed transparency images)


1. EXCELLENT video: [Polymaker: 3D Print Any Image - Lithophane Lightbox](https://www.youtube.com/watch?v=3i6UzTQTSZU)
    1. Recommended image to .stl lithophane converter tool: https://3dp.rocks/lithophane/
    1. Recommended settings (written in the descriptions under the video above):
        1. Image preparation:
            1. Crop your image to `3:2` width:height ratio
                1. Can be done in Gimp via Tools --> Transform Tools --> Crop, then select the "Tool Options" tab, check the box for "Fixed" Aspect ratio, and enter `3:2` into the box. Click and drag the right-sized box on the screen, and position it where you want it. Press <kbd>Enter</kbd> to complete the crop. 
                1. See: https://docs.gimp.org/en/gimp-tutorial-quickie-crop.html
            1. Save image as .jpg less than 1 MB in size
        1. Go here: https://3dp.rocks/lithophane/ --> choose "Outer Curve" lithophane type at the bottom
        1. Settings --> **Model Settings**:
            |                     |             |
            |---------------------|-------------|
            | Maximum Size:       | ~`150`~ mm [GS use `110` mm for small printers such as ToyBox]   |
            | Thickness:          | `2` mm      |
            | Border:             | `4` mm      |
            | Thinnest Layer:     | `0.8` mm    |
            | Vectors Per Pixel:  | ~`10`~ [GS use `4` instead in order to keep output .stl file size < 20 MB, which is required by the ToyBox printer]        |
            | Base/Stand Depth:   | `0`         |
            | Curve:              | `0`         |

            1. Size notes for a sample input .jpg which was 0.63 MB. Output .stl file (ToyBox requires < 20 MB) is:
                1. `10` vectors per pixel: 83.6 MB
                1. `7` vectors per pixel:  41.0 MB
                1. `5` vectors per pixel:  20.9 MB
                1. `4` vectors per pixel:  13.4 MB <-- so use this one to keep .stl file size < 20 MB

            ![image](https://user-images.githubusercontent.com/6842199/149876504-ffe7f9d8-eb96-48fb-b5b8-75000de131db.png)
        1. Settings --> **Image Settings**:
            |                     |             |
            |---------------------|-------------|
            | `Positive Image`    |             |  
            | `Mirror Image Off`  |             |
            | `Flip Image Off`    |             |
            | `Manual Refresh`    |             |
            | Repeat X Count:     | `1`         |
            | Repeat Y Count:     | `1`         |
            | `Mirror Repeat Off` |             |
            | `Flip Repeat Off`   |             |

            See: ![image](https://user-images.githubusercontent.com/6842199/149876696-49e2b3df-b1ef-450e-b173-275750b8d2b3.png)
        1. Click the "Model" tab --> "Refresh" button to do the conversion!
        1. Click the "Model" tab --> "Download" button to save the generated .stl file lithophane.

END

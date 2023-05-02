---
layout: page
title: RWTH Colors 
description: Collection of RWTH Aachen University's CD colors in various formats
img: assets/img/rwth-color-palette.png
importance: 1
category: Work
---

As part of my daily work I have to create a lot of plots and visualization and usually put quite some effort into them to make them look nice. Since colors are one important part of good visualizations, it is usually recommended to choose colors from a pre-defined color palette. Most plotting libraries and tools therefore usually have some default color palette and color cycle built-in that look nice and make such tools easily recognizable which is a good thing.

Since my university has its own color palette as part of a corporate design, I always try to use these colors in any of my projects.
The colors are provided in a PDF file as well as some templates for Microsoft Office and some other creative applications. To use them in tools like Python, usually the only choice to use them is to manually type in the HEX or RGB code in the desired plotting tool. This annoyed me as it is error prone and confusing as it is easy to forget which HEX code corresponds to which colors.

Therefore I created a small Python package that contains all of RWTH's colors as callable objects. I know that I am not the first research assistant that stumbled on this issue and created some kind of template or package. The existing packages, however, usually have some of these drawbacks:
- They simply provide some kind of `dict` and you need to know the correct key or color name respectively.
- They just provide `matplotlib` styles and don't make it possible to access the color codes directly to use them with other libraries

My package aims to solve both drawbacks and allow for a general easy use of the colors. The package can simply be installed using `pip install rwthcolors`. More information about the usage can be found on [GitHub](https://github.com/ifs-rwth-aachen/RWTH-Colors)

The repository furthermore contains the color definitions in some more formats (CSS, LaTeX, etc.)


<div class="row justify-content-sm-center">
    <div class="col-sm-8 mt-3 mt-md-0">
        {% include figure.html path="assets/img/plot.png" title="Example Plot" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm-4 mt-3 mt-md-0">
        {% include figure.html path="https://github.com/ifs-rwth-aachen/RWTH-Colors/raw/master/Python/rwth-colors/tests/output/palette.png" title="Color Palette" class="img-fluid rounded z-depth-1" %}
    </div>

</div>
<div class="caption">
    Matplotlib example plot and plot of RWTH CD color palette.
</div>

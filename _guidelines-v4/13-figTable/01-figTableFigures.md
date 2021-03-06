---
sectionid: figTableFigures
title: "Figures"
version: "v4"
---



 The [fig]({{ site.baseurl }}/{{ page.version }}/elements/fig.html){:.link_odd_elementSpec} element groups elements representing or containing graphic
information such as an illustration or figure. This element is modelled on the figure
element
in the Text Encoding Initiative (TEI). The [fig]({{ site.baseurl }}/{{ page.version }}/elements/fig.html){:.link_odd_elementSpec} element is used to
contain images, captions, and textual descriptions of the pictures. The images themselves
are
specified using the [graphic]({{ site.baseurl }}/{{ page.version }}/elements/graphic.html){:.link_odd_elementSpec} element, whose **@target** attribute
provides the location of an image. For example:

{% include plainExample.html example="examples/figTable/figTable-sample238.xml" valid="true" version=page.version %}

The graphic element may occur multiple times within the markup of the figure in order
to
indicate the availablity of different image formats or resolutions:

{% include plainExample.html example="examples/figTable/figTable-sample239.xml" valid="true" version=page.version %}




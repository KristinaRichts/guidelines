---
sectionid: usersymbolsReusableSymbols
title: "Defining Reusable Symbols"
version: "v3"
---



The [symbolDef]({{ site.baseurl }}/{{ page.version }}/elements/symbolDef.html){:.link_odd_elementSpec} element uses SVG markup or the aforementioned graphic
primitives to describe a symbol. A symbol definition may also use symbols defined
by other
[symbolDef]({{ site.baseurl }}/{{ page.version }}/elements/symbolDef.html){:.link_odd_elementSpec} elements by employing the [symbol]({{ site.baseurl }}/{{ page.version }}/elements/symbol.html){:.link_odd_elementSpec}
element.

<figure class="figure">{% include plainExample.html example="examples/userSymbols/userSymbols-sample345.xml" valid="true" version=page.version %}
   
   <figcaption class="figure-caption">Listing 1. Definition of a triangle percussion symbol using graphic primitives</figcaption>
</figure>

<figure class="figure"><img src="{{ site.baseurl }}/Images/modules/usersymbols/triangle.png" class="img-responsive"><figcaption class="figure-caption">Figure 53. Rendition of the triangle defined above</figcaption>
</figure>

<figure class="figure">{% include plainExample.html example="examples/userSymbols/userSymbols-sample346.xml" valid="true" version=page.version %}
   
   <figcaption class="figure-caption">Listing 2. Symbol composed of the symbol defined above and additional graphics primitives</figcaption>
</figure>

<figure class="figure"><img src="{{ site.baseurl }}/Images/modules/usersymbols/triangleWithStick.png" class="img-responsive"><figcaption class="figure-caption">Figure 54. Rendition of the composite triangle symbol</figcaption>
</figure>

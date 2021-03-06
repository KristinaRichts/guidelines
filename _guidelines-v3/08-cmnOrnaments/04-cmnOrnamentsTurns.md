---
sectionid: cmnOrnamentsTurns
title: "Turns"
version: "v3"
---



A turn is an ornament that typically consists of four notes: the upper neighbor of
the
principal note, the principal note, the lower neighbor, and the principal note again.


The presence of a turn is encoded with the [turn]({{ site.baseurl }}/{{ page.version }}/elements/turn.html){:.link_odd_elementSpec} element and its
attributes:




{% include specDesc.html version=page.version elem="turn" atts="att.turn.log/form att.turn.log/delayed" %}
{% include specDesc.html version=page.version elem="att.ornamentaccid" atts="att.ornamentaccid/accidlower att.ornamentaccid/accidupper" %}




It is recommended, but not required, to use the attribute **@form** to encode the
typology of the turn.


The attribute **@form** accepts the following values:


<table class="table table-striped">
   <thead>
      <tr>
         <th>Value</th>
         <th>Description</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>norm</td>
         <td> - usually corresponding to the symbol: <img src="{{ site.baseurl }}/Images/modules/cmnOrnaments/turn.png" class="graphic">. This turn is commonly
            performed beginning on a note higher than the principal note.
         </td>
      </tr>
      <tr>
         <td>inv</td>
         <td> - usually corresponding to the symbol: <img src="{{ site.baseurl }}/Images/modules/cmnOrnaments/inv_turn.png" class="graphic">. This turn is commonly
            performed beginning on a note lower than the principal note.
         </td>
      </tr>
   </tbody>
</table>



The following example shows the encoding of a simple turn:


<figure class="figure"><img src="{{ site.baseurl }}/Images/modules/cmnOrnaments/ex_turn.png" class="img-responsive"><figcaption class="figure-caption">Figure 33. Example of a simple turn.</figcaption>
</figure>
{% include plainExample.html example="examples/cmnOrnaments/cmnOrnaments-sample193.xml" valid="true" version=page.version %}


Turns can sometimes be performed after the principal note (usually on the second half
of the
beat, see <span class="bibl">Read 1979, p. 246</span>) and leading to the following event. To indicate
this, the turn symbol is typically written in between the principal note and the next.
These
kind of turns are encoded with the attribute **@delayed**.


The following example from Beethoven's piano sonata no. 1 in F minor, op. 2, no. 1,
mvmt. 2
demonstrates the encoding of turns with the **@delayed** attribute. Note that the
**@tstamp** attribute indicates the actual starting point in time, while
**@startid** points to the principal note.


<figure class="figure"><img src="{{ site.baseurl }}/Images/modules/cmnOrnaments/ex_turn_d.png" class="img-responsive"><figcaption class="figure-caption">Figure 34. Delayed turn.</figcaption>
</figure>
{% include plainExample.html example="examples/cmnOrnaments/cmnOrnaments-sample194.xml" valid="true" version=page.version %}


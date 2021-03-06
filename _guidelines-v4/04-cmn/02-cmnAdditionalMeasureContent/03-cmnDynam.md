---
sectionid: cmnDynam
title: "Dynamics in CMN"
version: "v4"
---



Common Music Notation provides two different methodologies for expressing the volume
of a
note, phrase, section, etc. The first is a verbal instruction providing such information
in
human language, possibly in an abbreviated form. An example is the word <span class="hi">piano</span>, indicating a quiet volume, often abbreviated as

<span class="hi">p</span>. In MEI, verbal instructions like this are encoded
using the [dynam]({{ site.baseurl }}/{{ page.version }}/elements/dynam.html){:.link_odd_elementSpec} element from the Shared module (see chapter 
<a class="link_ptr" title="Shared Elements, Models, and Attributes" href="{{ site.baseurl }}/{{ page.version }}/guidelines/shared.html">1 Shared Elements, Models, and Attributes</a>):

{% include plainExample.html example="examples/cmn/cmn-sample123.xml" valid="true" version=page.version %}


By convention, [dynam]({{ site.baseurl }}/{{ page.version }}/elements/dynam.html){:.link_odd_elementSpec} elements, like [slur]({{ site.baseurl }}/{{ page.version }}/elements/slur.html){:.link_odd_elementSpec} and
other elements belonging to the [model.controleventLike]({{ site.baseurl }}/{{ page.version }}/model-classes/model.controleventLike.html){:.link_odd} class,
are encoded at the end of the [measure]({{ site.baseurl }}/{{ page.version }}/elements/measure.html){:.link_odd_elementSpec} to which they belong. This
requires [dynam]({{ site.baseurl }}/{{ page.version }}/elements/dynam.html){:.link_odd_elementSpec} to be assigned to a certain [staff]({{ site.baseurl }}/{{ page.version }}/elements/staff.html){:.link_odd_elementSpec}
using the **@staff** attribute, whose value refers to the target element's
**@n** attribute. In the absence of other information, all layers within the staff
are assumed to have the same dynamic marking.

{% include plainExample.html example="examples/cmn/cmn-sample124.xml" valid="true" version=page.version %}


However, when the layers of a staff have different dynamic indications, the
**@layer** attribute may be used to associate a dynamic marking with a particular
layer:

{% include plainExample.html example="examples/cmn/cmn-sample125.xml" valid="false" version=page.version %}


A value in the range 0-127 may be assigned to a dynamic marking using the **@val**
attribute:

{% include plainExample.html example="examples/cmn/cmn-sample126.xml" valid="true" version=page.version %}


The location of a dynamic marking in relation to a staff may be specified using the
**@place** attribute, which may be given as *above*, *within*,
or *below* the staff:

{% include plainExample.html example="examples/cmn/cmn-sample127.xml" valid="true" version=page.version %}


Dynamics must also be associated with a particular time point in a measure, using
the
**@tstamp**, or with a particular event, using the **@startid** attribute.
Linking a control event with measures and events is discussed in section 
<a class="link_ptr" title="Timestamps and Durations" href="{{ site.baseurl }}/{{ page.version }}/guidelines/cmn.html#cmnTstamp">4.1.5 Timestamps and Durations</a>:

{% include plainExample.html example="examples/cmn/cmn-sample128.xml" valid="true" version=page.version %}

Dynamics which do not have an explicit endpoint are often referred to as
‘instantaneous’. On the other hand, some dynamic directions indicate a
continuous change that must have a defined end point. It is possible to specify the
logical
scope of continuous dynamic marks using the attributes **@tstamp2**, **@dur** or
**@endid**. In order to capture the fact that they continue until the first beat of
the next measure, the crescendi in the example above may be marked:

{% include plainExample.html example="examples/cmn/cmn-sample129.xml" valid="false" version=page.version %}


Any combination of **@tstamp**, **@startid**, **@tstamp2**, and
**@endid** attributes may be used to define the scope of a dynamic, although the
**@tstamp** and **@tstamp2** or the **@startid** and **@endid**
combinations are the most likely combinations. For example, the following alternatives
are
all possibilities for encoding up a crescendo. The choice of attributes is
often task or processor dependent.

{% include plainExample.html example="examples/cmn/cmn-sample130.xml" valid="false" version=page.version %}


All musical elements affected by the [dynam]({{ site.baseurl }}/{{ page.version }}/elements/dynam.html){:.link_odd_elementSpec} may be explicitly
specified using the **@plist** attribute, which contains **@xml:id** attribute
value references:

{% include plainExample.html example="examples/cmn/cmn-sample131.xml" valid="true" version=page.version %}


It is recommended that the list of references in **@plist** include all participants
in the dynamic marking, including the first and last notes as in the preceding example,
even
though they are duplicated by **@startid** and **@endid** attributes.


In addition to verbal instructions, Common Music Notation uses graphical symbols to
indicate ‘continuous’ dynamics. These crescendo and
decrescendo (or diminuendo) symbols are encoded in MEI using the
[hairpin]({{ site.baseurl }}/{{ page.version }}/elements/hairpin.html){:.link_odd_elementSpec} element. It also is a member of the [model.controleventLike]({{ site.baseurl }}/{{ page.version }}/model-classes/model.controleventLike.html){:.link_odd} class, which means it too is used just before the close of
a [measure]({{ site.baseurl }}/{{ page.version }}/elements/measure.html){:.link_odd_elementSpec} element, following the encoding of all staves. The required
attribute **@form** specifies the direction of the symbol by taking one of two
possible values: *cres* (growing louder) or *dim* (getting
softer).

{% include plainExample.html example="examples/cmn/cmn-sample132.xml" valid="true" version=page.version %}


Marking the logical extent of hairpins is possible using the same attributes as for
[dynam]({{ site.baseurl }}/{{ page.version }}/elements/dynam.html){:.link_odd_elementSpec}. The following example shows a hairpin that begins on the second
half of beat 2 (in the current measure) and ends on beat 1 (of the following measure).

{% include plainExample.html example="examples/cmn/cmn-sample133.xml" valid="true" version=page.version %}





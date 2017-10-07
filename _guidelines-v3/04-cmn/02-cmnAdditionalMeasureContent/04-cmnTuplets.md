---
sectionid: cmnTuplets
title: "Tuplets"
---



Tuplets indicate a localized change of meter; that is, a given duration in the regular
meter is divided between a group of notes with irregular (according to the current
meter)
rhythmic values. The most common tuplet is a so-called ‘triplet’, in
which three notes take the time normally occupied by two.

The relation of the tuplet to the underlying meter is specified using the **@num**
and **@numbase** attributes, where **@num** specifies the number of replacing
notes and **@numbase** specifies the number of notes *of the same duration*
to be replaced. For example, when three eighth notes replace one quarter note in common
time, **@num** takes a value of "3", whereas **@numbase** reads "2", because a
quarter note in common time is normally divided into two eighths. When three quarters
replace two in the same meter, **@numbase** also reads "2". The combination of these
attributes may be read as "3 in the time of 2" in either case.

The duration of the entire tuplet may be encoded using the usual ‘power of
2’ values, e.g., 1, 2, 4, etc., in the **@dur** attribute, and the
**@dots** attribute, if necessary.

{% include _plainExample.html example="./v3/examples/cmn/cmn-sample134.xml" valid="true" %}




Tuplets are often highlighted using brackets above or below the affected notes. The
presence and position of these brackets can be encoded using the **@bracket.place**
(above / below) and **@bracket.visible** (true / false) attributes.

Usually, however, tuplets are rendered with a bracket (**@bracket.visible**="true")
and a single number (**@num.format**="count" and **@num.visible**="true").
However, the number-to-numbase ratio may be provided in addition to, or in some cases
as a
replacement for, the bracket. The **@num.format** attribute indicates whether a plain
number (the value of **@num**) or a ratio (comprised of **@num** and
**@numbase**, e.g., "3:2") should be displayed and **@num.visible** indicates
the general presence of such a number. 



In addition to <a class="link_odd_elementSpec" href="/v3/elements/note">note</a> elements, 
<a class="link_odd_elementSpec" href="/v3/elements/tuplet">tuplet</a> may
contain other elements, such as 
<a class="link_odd_elementSpec" href="/v3/elements/rest">rest</a> or 
<a class="link_odd_elementSpec" href="/v3/elements/space">space</a>,
to match the content of a source document or an intended rendering. In particular,
the 
<a class="link_odd_elementSpec" href="/v3/elements/beam">beam</a> element is allowed so that custom beaming may be indicated, e.g., a
septuplet may be divided into a group of three plus a group of four
notes.



The 
<a class="link_odd_elementSpec" href="/v3/elements/tuplet">tuplet</a> element may also be used for repetition of the same pitch;
that is, a single note or chord may be the only content of the tuplet. In some cases,
optical music recognition software may treat these instances as bowed tremolandi due
to the
knowledge of the complete semantics of the notation at the time of recognition. However,
marking these as tuplets is the recommended practice.


In some situations, a tuplet is made up of events in different measures. As this raises
the
issue of non-concurrent hierarchies, it is not possible to encode such situations
with the

<a class="link_odd_elementSpec" href="/v3/elements/tuplet">tuplet</a> element described above. Therefore, MEI offers the 
<a class="link_odd_elementSpec" href="/v3/elements/tupletSpan">tupletSpan</a> element, which is member of the 
<a class="link_odd" href="/v3/model-classes/model.controleventLike">model.controleventLike</a> class. It is nested inside of 
<a class="link_odd_elementSpec" href="/v3/elements/measure">measure</a>, following all the measure's 
<a class="link_odd_elementSpec" href="/v3/elements/staff">staff</a> children. It uses
the same attributes as 
<a class="link_odd_elementSpec" href="/v3/elements/tuplet">tuplet</a> to describe tuplets, but instead of
nesting all affected notes inside itself, it references the **@xml:id** values of all
affected notes in its **@plist** attribute and the initial and terminal notes of the
tuplet using **@startid** and **@endid** attributes. This configuration allows
tuplets to cross measure boundaries. The following example demonstrates a typical
example of
such hierarchy-crossing tuplets:

{% include _plainExample.html example="./v3/examples/cmn/cmn-sample135.xml" valid="true" %}


---
sectionid: cmnTstamp
title: "Timestamps and Durations"
version: "v4"
---



MEI offers multiple ways of defining onsets and offsets of timed musical events such
as
notes and slurs. The most common and most musician-friendly approach to this is through
the
use of a combination of the attributes **@tstamp** and **@dur**, which are made
available by the attribute classes [att.timestamp.musical]({{ site.baseurl }}/{{ page.version }}/attribute-classes/att.timestamp.musical.html){:.link_odd}
(inherited by [att.controlevent]({{ site.baseurl }}/{{ page.version }}/attribute-classes/att.controlevent.html){:.link_odd}) and [att.duration.musical]({{ site.baseurl }}/{{ page.version }}/attribute-classes/att.duration.musical.html){:.link_odd}, both from the shared module.

The timestamp (**@tstamp**) of a musical event is calculated in relation
to the meter of the current measure and resembles the so-called ‘beat’.
In a common time measure with four quarter notes, the timestamp of each quarter equals
its
beat position in the measure: The first quarter has a timestamp of 1, the second has
a
timestamp of 2, and so on. MEI defines the value of **@tstamp** as a real number; the
second eighth note position in a measure would thus be represented by the value of
"1.5".
The range of possible values is defined as starting with zero and ending with the
number of
metrical units in a measure (the ‘numerator’ in a time signature) + 1.
This allows the capture of all graphical positions starting from the left barline
('0') and
ending with the right barline of the measure ('5', in the case of 4/4 time).

For expressing durations, MEI offers the **@dur** attribute. This attribute is
described in section <a class="link_ptr" title="Basic Usage of Notes in CMN" href="{{ site.baseurl }}/{{ page.version }}/guidelines/cmn.html#cmnNotesBasic">4.1.4.1.1 Basic Usage of Notes in CMN</a>.

For ‘spanning’ elements like slurs, which are members of the [model.controleventLike]({{ site.baseurl }}/{{ page.version }}/model-classes/model.controleventLike.html){:.link_odd} class, it is often more intuitive to record
two timestamps – one for the onset of the event and one for its termination. Because
the
termination of the event may be in a succeeding measure, the second timestamp
(**@tstamp2**) has a slightly different datatype than the one marking the initiation
of the event. Its datatype is constrained to values following the formula "
<span class="hi">x</span>m+
<span class="hi">y</span>", where 
<span class="hi">x</span> is the number of full
measures that this particular feature lasts (or the number of bar lines crossed) and

<span class="hi">y</span> is the timestamp in the target measure where the feature ends. The
timestamp is expressed using the same logic as described above. For example, a value
of
"0m+3" in 4/4 time indicates that the element bearing this attribute, a slur for example,
ends on beat 3 of the same measure where it started. A value of "1m+1.5" would indicate
an
end on the second eighth note of the following measure. In 6/8 time, the value "2m+3"
means
that the feature ends two measures later on the third eighth note.


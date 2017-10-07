---
sectionid: edittransOmission
title: "Omissions, Unclear Readings, Damage, and Supplied Readings"
---



Encoders may choose to omit parts of the source for reasons ranging from illegibility,
(making transcription difficult or impossible), to editorial policy, e.g., systematic
exclusion of poetry or prose from an encoding. The full details of the policy decisions
concerned should be documented in the MEI header (see section <a class="link_ptr" title="Encoding Description" href="/v3/guidelines/header#headerEncodingDescription">2.2 Encoding Description</a>). Each place in the text at which omission has taken
place should be marked with a 
<a class="link_odd_elementSpec" href="/v3/elements/gap">gap</a> element, optionally with further
information about the reason for the omission, its extent, and the person or agency
responsible for it, as in the following examples:

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample221.xml" valid="true" %}

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample222.xml" valid="true" %}


Note that the extent of the gap may be marked precisely using attributes **@unit**
and **@quantity**, or more descriptively using the **@extent** attribute.

Unlike TEI, MEI does not offer a *desc* element for further description of
the reason for a gap. Instead, an 
<a class="link_odd_elementSpec" href="/v3/elements/annot">annot</a> may refer to the gap via its
**@startid**, **@endid**, or **@plist** attributes and provide
additional information.

The 
<a class="link_odd_elementSpec" href="/v3/elements/unclear">unclear</a> element is used to mark passages in the original which
cannot be read with confidence, or about which the transcriber is uncertain for other
reasons, as for example when transcribing a illegible source. Its **@reason** and
**@resp** attributes are used, as with the 
<a class="link_odd_elementSpec" href="/v3/elements/gap">gap</a> element, to
indicate the cause of uncertainty and the person responsible for the conjectured
reading.

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample223.xml" valid="true" %}


Where the difficulty in transcription arises from an identifiable cause, the
**@agent** attribute signifies the causative agent. The **@cert** attribute
signifies the degree of certainty ascribed to the transcription of the text contained
within
the 
<a class="link_odd_elementSpec" href="/v3/elements/unclear">unclear</a> element. Where the difficulty in transcription arises from
action (partial deletion, etc.) assignable to an identifiable hand, the **@hand**
attribute may record the hand responsible for the action.

When the reason for a gap in the encoding is damage of the document carrier (the paper
on
which the document is written, for example), the 
<a class="link_odd_elementSpec" href="/v3/elements/damage">damage</a> element should
be used instead of the 
<a class="link_odd_elementSpec" href="/v3/elements/gap">gap</a> element. In the case of damage resulting
from an identifiable cause, the **@agent** attribute signifies the causative agent.
The **@degree** attribute signifies the degree of damage according to a convenient
scale. A 
<a class="link_odd_elementSpec" href="/v3/elements/damage">damage</a> tag with this attribute should only be used where the
text may be read with some confidence; data supplied from other sources should be
tagged as

<a class="link_odd_elementSpec" href="/v3/elements/supplied">supplied</a>. The **@extent** attribute indicates approximately
how much text is in the damaged area, in notes, measures, inches, or any appropriate
unit,
where this cannot be deduced from the contents of the tag. For example, the damage
may span
structural divisions in the text so that the tag must then be empty of content. In
the case
of damage (deliberate defacement, etc.) assignable to an identifiable hand, the
**@hand** attribute signifies the hand responsible for the damage.

Sometimes the editor provides information not present in the source material. These
conjectures or emendations are marked up in MEI using the 
<a class="link_odd_elementSpec" href="/v3/elements/supplied">supplied</a>
element.

The following example demonstrates the use of the 
<a class="link_odd_elementSpec" href="/v3/elements/supplied">supplied</a> element in
combination with 
<a class="link_odd_elementSpec" href="/v3/elements/gap">gap</a> within 
<a class="link_odd_elementSpec" href="/v3/elements/subst">subst</a>:

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample224.xml" valid="true" %}


When the presumed loss of text arises from an identifiable cause, **@agent**
signifies the causative agent. When the presumed loss of text arises from action (partial
deletion, etc.) assignable to an identifiable hand, the **@hand** attribute signifies
the hand responsible for the action. The **@reason** attribute indicates why the text
has to be supplied, e.g. 'overbinding', 'faded ink', 'lost folio', 'omitted in original',
etc. The **@source** attribute contains the source of the supplied text. The editor(s)
responsible for supplied material may be recorded in the **@resp** attribute. The
value of **@resp** must point to one or more identifiers declared in the document
header. The **@cert** attribute signifies the degree of certainty ascribed to the
supplied material.


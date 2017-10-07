---
sectionid: headerRevisionDescription
title: "Revision Description"
---



The final sub-element of the MEI header, the <a class="link_odd_elementSpec" href="/v3/elements/revisionDesc">revisionDesc</a> element,
provides a detailed change log in which each change made to a text may be recorded.
Its use is
optional but highly recommended. It provides essential information for the administration
of
large numbers of files which are being updated, corrected, or otherwise modified as
well as
extremely useful documentation for files being passed from researcher to researcher
or system
to system. Without change logs, it is easy to confuse different versions of a file,
or to
remain unaware of small but important changes made in the file by some earlier link
in the
chain of distribution. No change should be made in any MEI-conformant file without
corresponding entries being made in the change log.



{% include _specDesc.html key="revisionDesc" atts="" %}
{% include _specDesc.html key="change" atts="" %}




The main purpose of the revision description is to record changes in the text to which
a
header is prefixed. However, it is recommended practice to include entries also for
significant changes in the header itself (other than the revision description itself,
of
course). At the very least, an entry should be supplied indicating the date of creation
of the
header.

The log consists of a list of 
<a class="link_odd_elementSpec" href="/v3/elements/change">change</a> elements, each of which contains a
detailed description of the changes made. If a number is to be associated with one
or more
changes (for example, a revision number), the **@n** attribute may be used to indicate
it. The person responsible for the change and the date of the change may be indicated
by the

<a class="link_odd_elementSpec" href="/v3/elements/respStmt">respStmt</a> and 
<a class="link_odd_elementSpec" href="/v3/elements/date">date</a> elements. The description of
the change itself is contained within the 
<a class="link_odd_elementSpec" href="/v3/elements/changeDesc">changeDesc</a> element, which can
hold one or more paragraphs.

It is recommended to give changes in reverse chronological order, most recent first.

For example:

{% include _plainExample.html example="./v3/examples/header/header-sample075.xml" valid="true" %}

A slightly shorter form for recording changes is also available when a the date of
the change
can be described by a single date in a standard ISO form and when the name of the
agent(s)
responsible for the change, encoded elsewhere in the header, can be referred to by
one or more
URIs given in the **@resp** attribute. For example:

{% include _plainExample.html example="./v3/examples/header/header-sample076.xml" valid="true" %}

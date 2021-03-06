---
sectionid: headerWorkLanguage
title: "Language Usage"
version: "v4"
---



The [langUsage]({{ site.baseurl }}/{{ page.version }}/elements/langUsage.html){:.link_odd_elementSpec} element is used within the [workDesc]({{ site.baseurl }}/{{ page.version }}/elements/workDesc.html){:.link_odd_elementSpec} element to describe the languages, sublanguages, dialects, etc. represented
within a work. It contains one or more [language]({{ site.baseurl }}/{{ page.version }}/elements/language.html){:.link_odd_elementSpec} elements, each of
which provides information about a single language.



{% include specDesc.html version=page.version elem="langUsage" atts="" %}
{% include specDesc.html version=page.version elem="language" atts="" %}



A [language]({{ site.baseurl }}/{{ page.version }}/elements/language.html){:.link_odd_elementSpec} element may be supplied for each different language used
in a document. If used, its **@xml:id** attribute should specify an appropriate
language identifier. This is particularly important if extended language identifiers
have
been used as the value of @xml:lang attributes elsewhere in the document.

Here is an example of the use of this element:

{% include plainExample.html example="examples/header/header-sample054.xml" valid="false" version=page.version %}


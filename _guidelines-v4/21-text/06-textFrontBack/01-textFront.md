---
sectionid: textFront
title: "Front Matter"
version: "v4"
---



By ‘front matter’ these Guidelines mean distinct sections of a text
(usually, but not necessarily, a printed one), prefixed to it by way of introduction
or
identification as a part of its production. Features such as title pages or prefaces
are
clear examples; a less definite case might be the prologue attached to a dramatic
work. The
front matter of an encoded text should not be confused with the MEI header described
in
chapter <a class="link_ptr" title="The MEI Header" href="{{ site.baseurl }}/{{ page.version }}/guidelines/header.html">2 The MEI Header</a>, which provides metadata for the entire file.

An encoder may choose simply to ignore the front matter in a text, if the original
presentation of the work is of no interest. No specific tags are provided for the
various
kinds of subdivision which may appear within front matter: instead, generic [div]({{ site.baseurl }}/{{ page.version }}/elements/div.html){:.link_odd_elementSpec} (“division”) elements may be used, which should not be confused with [mdiv]({{ site.baseurl }}/{{ page.version }}/elements/mdiv.html){:.link_odd_elementSpec} (“musical division”) elements. The following suggested values for
the **@type** attribute may be used to distinguish various kinds of division
characteristic of front matter:


<table class="table table-striped table-hover">
   <thead>
      <tr>
         <th>Value</th>
         <th>Description</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>'preface' – </td>
         <td>A foreword or preface addressed to the reader in which the author or publisher
            explains the content, purpose, or origin of the text. 
         </td>
      </tr>
      <tr>
         <td>'ack' – </td>
         <td>A formal declaration of acknowledgement by the author in which persons and
            institutions are thanked for their part in the creation of a text.
         </td>
      </tr>
      <tr>
         <td>'dedication' – </td>
         <td>A formal offering or dedication of a text to one or more persons or institutions by
            the author.
         </td>
      </tr>
      <tr>
         <td>'abstract' – </td>
         <td>A summary of the content of a text as continuous prose.</td>
      </tr>
      <tr>
         <td>'contents' – </td>
         <td>A table of contents, specifying the structure of a work and listing its constituents.
            The list element should be used to mark its structure.
         </td>
      </tr>
      <tr>
         <td>'frontispiece' – </td>
         <td>A pictorial frontispiece, possibly including some text.</td>
      </tr>
   </tbody>
</table>
The following extended example demonstrates how various parts of the front matter
of a text
may be encoded. The front part begins with a title page, which is presented in section

<a class="link_ptr" title="Title Pages" href="{{ site.baseurl }}/{{ page.version }}/guidelines/text.html#textTitlePages">21.6.2 Title Pages</a>, below. This is followed by a dedication and a preface, each of
which is encoded as a distinct div:

{% include plainExample.html example="examples/text/text-sample338.xml" valid="true" version=page.version %}

The front matter concludes with another [div]({{ site.baseurl }}/{{ page.version }}/elements/div.html){:.link_odd_elementSpec} element, shown in the
next example, this time containing a table of contents, which contains a [list]({{ site.baseurl }}/{{ page.version }}/elements/list.html){:.link_odd_elementSpec} element (as described in chapter 
<a class="link_ptr" title="Lists" href="{{ site.baseurl }}/{{ page.version }}/guidelines/text.html#textLists">21.3 Lists</a>). Note the use of
the [ptr]({{ site.baseurl }}/{{ page.version }}/elements/ptr.html){:.link_odd_elementSpec} element to provide page-references: the implication here is
that the target identifiers (song1, song2, etc.) will correspond with identifiers
used for
the [mdiv]({{ site.baseurl }}/{{ page.version }}/elements/mdiv.html){:.link_odd_elementSpec} elements containing the individual songs. (For a description
of the [ptr]({{ site.baseurl }}/{{ page.version }}/elements/ptr.html){:.link_odd_elementSpec} element, see chapter 
<a class="link_ptr" title="Pointers and References" href="{{ site.baseurl }}/{{ page.version }}/guidelines/ptrRef.html">19 Pointers and References</a>.)

{% include plainExample.html example="examples/text/text-sample339.xml" valid="true" version=page.version %}

Alternatively, the pointers in the table of contents might link to the page breaks
at which
a song begins, assuming that these have been included in the markup:

{% include plainExample.html example="examples/text/text-sample340.xml" valid="true" version=page.version %}


---
sectionid: edittransAbbrev
title: "Abbreviations"
---



MEI offers methods for marking abbreviations in prose, as in the following example:

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample207.xml" valid="true" %}

or abbreviations in the music itself, as in the following example:

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample208.xml" valid="true" %}



The type attribute may be used to classify the abbreviation according to a convenient
typology. Sample values include:

<table class="table table-striped table-hover">
   <thead>
      <tr>
         <th>name</th>
         <th>genre</th>
      </tr>
   </thead>
   <tbody>
      <tr>
         <td>suspension - </td>
         <td> the abbreviation provides the first letter(s) of the word or phrase, omitting the
            remainder;
         </td>
      </tr>
      <tr>
         <td>contraction -</td>
         <td> the abbreviation omits some letter(s) in the middle;</td>
      </tr>
      <tr>
         <td>brevigraph - </td>
         <td> the abbreviation comprises a special symbol or mark;</td>
      </tr>
      <tr>
         <td>superscription - </td>
         <td> the abbreviation includes writing above the line;</td>
      </tr>
      <tr>
         <td>acronym - </td>
         <td> the abbreviation comprises the initial letters of the words of a phrase;</td>
      </tr>
      <tr>
         <td>title -</td>
         <td> the abbreviation is for a title of address (Dr, Ms, Mr, ...);</td>
      </tr>
      <tr>
         <td>organization - </td>
         <td> the abbreviation is for the name of an organization;</td>
      </tr>
      <tr>
         <td>geographic - </td>
         <td> the abbreviation is for a geographic name.</td>
      </tr>
   </tbody>
</table>

This tag is the mirror image of the 
<a class="link_odd_elementSpec" href="/v3/elements/expan">expan</a> tag (not to be confused with
the 
<a class="link_odd_elementSpec" href="/v3/elements/expansion">expansion</a> element described in 
<a class="link_ptr" title="Content of Musical Divisions" href="/v3/guidelines/shared#sharedMdivContent">1.1.2.3 Content of Musical Divisions</a>).
Both 
<a class="link_odd_elementSpec" href="/v3/elements/abbr">abbr</a> and 
<a class="link_odd_elementSpec" href="/v3/elements/expan">expan</a> allow the encoder to
transcribe an abbreviation and its expansion. In the case of 
<a class="link_odd_elementSpec" href="/v3/elements/abbr">abbr</a>, the
original is transcribed as the content of the element and the expansion as an attribute
value,
while 
<a class="link_odd_elementSpec" href="/v3/elements/expan">expan</a> reverses this. The choice between the two is up to the user.
For example:

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample209.xml" valid="false" %}


The 
<a class="link_odd_elementSpec" href="/v3/elements/abbr">abbr</a> tag is not required; if appropriate, the encoder may
transcribe abbreviations in the source text silently, without tagging them. If abbreviations
are not transcribed directly but expanded silently, then the MEI header should indicate
this
is the case. The **@cert** attribute signifies the degree of certainty ascribed to the
expansion of the abbreviation. The **@expan** attribute gives an expansion of the
abbreviation. The **@resp** attribute contains an ID reference to an element containing
the name of the editor or transcriber responsible for supplying the expansion of the
abbreviation.

When the content of the **@abbr** or **@expan** attributes requires additional
markup, an attribute cannot be used. In this case, the abbreviated and expanded forms
must be
presented within elements. Furthermore, as alternatives to each other, the 
<a class="link_odd_elementSpec" href="/v3/elements/abbr">abbr</a> and 
<a class="link_odd_elementSpec" href="/v3/elements/expan">expan</a> elements must be wrapped by the 
<a class="link_odd_elementSpec" href="/v3/elements/choice">choice</a> element, as described above. The previous example, where the 'o:' in 'pno:' is
written as superscript, would be encoded as:

{% include _plainExample.html example="./v3/examples/editTrans/editTrans-sample210.xml" valid="true" %}



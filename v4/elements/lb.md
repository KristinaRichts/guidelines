---
layout: sidebar
sidebar: s1
version: "v4"
title: "lb"

---

<div class="elementSpec">
   <h3 id="lb">&lt;lb&gt;</h3>
   <table class="wovenodd">
      <tr>
         <td colspan="2" class="wovenodd-col2">(line break) – An empty formatting element that forces text to begin on a new line.</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Module</strong></td>
         <td class="wovenodd-col2">MEI.shared</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Attributes</strong></td>
         <td class="wovenodd-col2">
            <table class="table table-striped">
               <thead>
                  <tr>
                     <th></th>
                  </tr>
               </thead>
               <tbody>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@class</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Contains one or more URIs which denote classification terms that apply to the entity
                              bearing this attribute.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.classed.html">att.classed</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@copyof</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Points to an element of which the current element is a copy.</span>
                           Value conforms to <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.linking.html">att.linking</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@corresp</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Used to point to other elements that correspond to this one in a generic
                              fashion.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.linking.html">att.linking</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@facs</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Permits the current element to reference a facsimile surface or image zone which
                              corresponds to it.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.facsimile.html">att.facsimile</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@func</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">States whether the line break follows a single line or a line group.</span>
                           Allowed values are:
                           "<span style="font-weight: 500;">line</span>" <i>(Follows a verse line.)</i>,  "<span style="font-weight: 500;">group</span>" <i>(Follows a group of verse lines.)</i><span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/lb.html">lb</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@label</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Captures text to be used to generate a label for the element to which it's attached,
                              a
                              "tool tip" or prefatory text, for example. Should not be used to record document
                              content.</span>
                           Value of datatype <span style="font-weight: 500;">string</span>.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.labelled.html">att.labelled</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@n</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Provides a number-like designation that indicates an element's position in a sequence
                              of similar elements. May not contain space characters.</span>
                           Value of datatype <span style="font-weight: 500;">
                              a string matching the following regular expression: "(\p{L}|\p{N}|\p{P}|\p{S})*"
                              </span>.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.nNumberLike.html">att.nNumberLike</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@next</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Used to point to the next event(s) in a user-defined collection.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.linking.html">att.linking</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@prev</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Points to the previous event(s) in a user-defined collection.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.linking.html">att.linking</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@sameas</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Points to an element that is the same as the current element but is not a literal
                              copy
                              of the current element.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.linking.html">att.linking</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@source</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Contains a list of one or more pointers indicating the sources which attest to a given
                              reading. Each value should correspond to the ID of a <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/source.html">source</a> element
                              located in the document header.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.source.html">att.source</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@synch</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Points to elements that are synchronous with the current element.</span>
                           One or more values from<a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.linking.html">att.linking</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@type</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Designation which characterizes the element in some sense, using any convenient
                              classification scheme or typology that employs single-token labels.</span>
                           One or more values of datatype <span style="font-weight: 500;">NMTOKEN</span>, separated by spaces.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.typed.html">att.typed</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@xml:base</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Provides a base URI reference with which applications can resolve relative URI
                              references into absolute URI references.</span>
                           Value conforms to <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.basic.html">att.basic</a></span></div>
                     </td>
                  </tr>
                  <tr>
                     <td>
                        <div class="attributeDef"><span class="attribute"><strong>@xml:id</strong></span><span class="attributeUsage">(optional)</span><span class="attributeDesc">Regularizes the naming of an element and thus facilitates building links between it
                              and other resources. Each id attribute within a document must have a unique value.</span>
                           Value of datatype <span style="font-weight: 500;">ID</span>.
                           <span class="attributeClasses"><a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.id.html">att.id</a></span></div>
                     </td>
                  </tr>
               </tbody>
            </table>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Member of</strong></td>
         <td class="wovenodd-col2">
            <div class="parent"><a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/model-classes/model.lbLike.html">model.lbLike</a></div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Contained by</strong></td>
         <td class="wovenodd-col2">
            <div class="parent">
               <div class="specChildren">
                  <div class="specChild"><span class="specChildModule">MEI.cmn</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/attacca.html">attacca</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/gliss.html">gliss</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/ligatureSpan.html">ligatureSpan</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/mNum.html">mNum</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/octave.html">octave</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/reh.html">reh</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.critapp</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/lem.html">lem</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/rdg.html">rdg</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.drama</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/sp.html">sp</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/stageDir.html">stageDir</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.edittrans</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/abbr.html">abbr</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/add.html">add</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/corr.html">corr</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/cpMark.html">cpMark</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/damage.html">damage</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/del.html">del</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/expan.html">expan</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/orig.html">orig</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/reg.html">reg</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/restore.html">restore</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/sic.html">sic</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/supplied.html">supplied</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/unclear.html">unclear</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.figtable</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/figDesc.html">figDesc</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/td.html">td</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/th.html">th</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.fingering</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/fing.html">fing</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.harmony</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/f.html">f</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/harm.html">harm</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.header</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/altId.html">altId</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/byline.html">byline</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/contentItem.html">contentItem</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/dedication.html">dedication</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/hand.html">hand</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/language.html">language</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/price.html">price</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/provenance.html">provenance</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/soundChan.html">soundChan</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.lyrics</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/refrain.html">refrain</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/verse.html">verse</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/volta.html">volta</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.namesdates</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/addName.html">addName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/bloc.html">bloc</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/corpName.html">corpName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/country.html">country</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/district.html">district</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/famName.html">famName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/foreName.html">foreName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/genName.html">genName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/geogFeat.html">geogFeat</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/geogName.html">geogName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/nameLink.html">nameLink</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/periodName.html">periodName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/persName.html">persName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/region.html">region</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/roleName.html">roleName</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/settlement.html">settlement</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/street.html">street</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/styleName.html">styleName</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.ptrref</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/ref.html">ref</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.shared</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/actor.html">actor</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/addrLine.html">addrLine</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/annot.html">annot</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/arranger.html">arranger</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/author.html">author</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/bibl.html">bibl</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/biblScope.html">biblScope</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/caption.html">caption</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/cb.html">cb</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/colLayout.html">colLayout</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/composer.html">composer</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/contributor.html">contributor</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/creation.html">creation</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/date.html">date</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/dedicatee.html">dedicatee</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/depth.html">depth</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/desc.html">desc</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/dimensions.html">dimensions</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/dir.html">dir</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/distributor.html">distributor</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/div.html">div</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/dynam.html">dynam</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/edition.html">edition</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/editor.html">editor</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/extent.html">extent</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/funder.html">funder</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/genre.html">genre</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/head.html">head</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/height.html">height</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/identifier.html">identifier</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/imprint.html">imprint</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/label.html">label</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/labelAbbr.html">labelAbbr</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/lb.html">lb</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/librettist.html">librettist</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/lyricist.html">lyricist</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/name.html">name</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/num.html">num</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/ornam.html">ornam</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/p.html">p</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/pgFoot.html">pgFoot</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/pgFoot2.html">pgFoot2</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/pgHead.html">pgHead</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/pgHead2.html">pgHead2</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/publisher.html">publisher</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/pubPlace.html">pubPlace</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/recipient.html">recipient</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/rend.html">rend</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/repository.html">repository</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/resp.html">resp</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/role.html">role</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/roleDesc.html">roleDesc</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/series.html">series</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/speaker.html">speaker</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/sponsor.html">sponsor</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/stack.html">stack</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/syl.html">syl</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/symbol.html">symbol</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/tempo.html">tempo</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/term.html">term</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/textLang.html">textLang</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/titlePage.html">titlePage</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/width.html">width</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.text</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/argument.html">argument</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/back.html">back</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/epigraph.html">epigraph</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/front.html">front</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/imprimatur.html">imprimatur</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/l.html">l</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/li.html">li</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/quote.html">quote</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/seg.html">seg</a></span></div>
                  <div class="specChild"><span class="specChildModule">MEI.usersymbols</span><span class="specChildElements"><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/anchoredText.html">anchoredText</a> <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/line.html">line</a></span></div>
               </div>
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>May contain</strong></td>
         <td class="wovenodd-col2">
            <div class="specChild"><span class="specChildModule">Empty</span><span class="specChildElements"></span></div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Declaration</strong></td>
         <td class="wovenodd-col2">
            <div class="code" xml:space="preserve" data-lang="ODD"><code>
                  <div class="indent1 indent"><span data-indentation="1" class="element">&lt;classes&gt;</span>
                     
                     <div class="indent2 indent"><span data-indentation="2" class="element">&lt;memberOf
                           <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.common.html">att.common</a>"</span></span>/&gt;</span></div>
                     
                     <div class="indent2 indent"><span data-indentation="2" class="element">&lt;memberOf
                           <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.facsimile.html">att.facsimile</a>"</span></span>/&gt;</span></div>
                     
                     <div class="indent2 indent"><span data-indentation="2" class="element">&lt;memberOf
                           <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.source.html">att.source</a>"</span></span>/&gt;</span></div>
                     
                     <div class="indent2 indent"><span data-indentation="2" class="element">&lt;memberOf
                           <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/model-classes/model.lbLike.html">model.lbLike</a>"</span></span>/&gt;</span></div>
                     <span data-indentation="1" class="element">&lt;/classes&gt;</span></div>
                  <div class="indent1 indent"><span data-indentation="1" class="element">&lt;content&gt;</span>
                     
                     <div class="indent2 indent"><span data-indentation="2" class="element">&lt;rng:empty/&gt;</span></div>
                     <span data-indentation="1" class="element">&lt;/content&gt;</span></div></code></div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Remarks</strong></td>
         <td class="wovenodd-col2">
            <p>The <span class="att">n</span> attribute should be used to record a number associated with this textual
               line. See comment on <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/verse.html">verse</a> element for description of <span class="att">func</span>
               attribute. Do not confuse this element with the <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/sb.html">sb</a> element, which
               performs a similar function for musical notation.This element is modelled on an element
               in the Text Encoding Initiative (TEI) standard.
            </p>
         </td>
      </tr>
   </table>
</div>
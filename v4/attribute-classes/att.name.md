---
layout: sidebar
sidebar: s1
version: "v4"
title: "att.name"

---

<div class="classSpec att">
   <h3 id="att.name">att.name</h3>
   <table class="wovenodd">
      <tr>
         <td colspan="2" class="wovenodd-col2">Attributes shared by names.</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Module</strong></td>
         <td class="wovenodd-col2">MEI.shared</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Members</strong></td>
         <td class="wovenodd-col2">
            <div class="parent">
               <div><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/addName.html">addName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/bloc.html">bloc</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/corpName.html">corpName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/country.html">country</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/district.html">district</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/famName.html">famName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/foreName.html">foreName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/genName.html">genName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/geogFeat.html">geogFeat</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/geogName.html">geogName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/nameLink.html">nameLink</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/periodName.html">periodName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/persName.html">persName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/region.html">region</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/roleName.html">roleName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/settlement.html">settlement</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/styleName.html">styleName</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/name.html">name</a>, <a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/repository.html">repository</a> (direct members of att.name)
               </div>
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Attributes</strong></td>
         <td class="wovenodd-col2"></td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Declaration</strong></td>
         <td class="wovenodd-col2">
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;classes&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;memberOf
                        <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.authorized.html">att.authorized</a>"</span></span>/&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;memberOf
                        <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.datable.html">att.datable</a>"</span></span>/&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;memberOf
                        <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.filing.html">att.filing</a>"</span></span>/&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/classes&gt;</span></div>
            </div>
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;attDef <span class="attribute">ident=</span><span class="attributevalue">"nymref"</span> <span class="attribute">usage=</span><span class="attributevalue">"opt"</span>&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;desc&gt;</span>Used to record a pointer to the regularized form of the name elsewhere in the
                     document.<span data-indentation="2" class="element">&lt;/desc&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;datatype <span class="attribute">maxOccurs=</span><span class="attributevalue">"1"</span> <span class="attribute">minOccurs=</span><span class="attributevalue">"1"</span>&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:ref
                           
                           <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.URI.html">data.URI</a>"</span></span>
                           /&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/datatype&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;constraintSpec <span class="attribute">ident=</span><span class="attributevalue">"check_nymrefTarget"</span> <span class="attribute">scheme=</span><span class="attributevalue">"isoschematron"</span>&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;constraint&gt;</span>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;sch:rule <span class="attribute">context=</span><span class="attributevalue">"@nymref"</span>&gt;</span>
                           
                           <div class="indent5 indent"><span data-indentation="5" class="element">&lt;sch:assert <span class="attribute">role=</span><span class="attributevalue">"warning"</span> <span class="attribute">test=</span><span class="attributevalue">"not(normalize-space(.) eq '')"</span>&gt;</span>@nymref attribute
                              should have content.<span data-indentation="5" class="element">&lt;/sch:assert&gt;</span></div>
                           
                           <div class="indent5 indent"><span data-indentation="5" class="element">&lt;sch:assert <span class="attribute">role=</span><span class="attributevalue">"warning"</span> <span class="attribute">test=</span><span class="attributevalue">"every $i in tokenize(., '\s+') satisfies substring($i,2)=//mei:*/@xml:id"</span>&gt;</span>The
                              value in @nymref should correspond to the @xml:id attribute of an
                              element.<span data-indentation="5" class="element">&lt;/sch:assert&gt;</span></div>
                           <span data-indentation="4" class="element">&lt;/sch:rule&gt;</span></div>
                        <span data-indentation="3" class="element">&lt;/constraint&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/constraintSpec&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/attDef&gt;</span></div>
            </div>
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;attDef <span class="attribute">ident=</span><span class="attributevalue">"role"</span> <span class="attribute">usage=</span><span class="attributevalue">"opt"</span>&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;desc&gt;</span>Used to specify further information about the entity referenced by this name, for
                     example, the occupation of a person or the status of a place.<span data-indentation="2" class="element">&lt;/desc&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;datatype <span class="attribute">maxOccurs=</span><span class="attributevalue">"1"</span> <span class="attribute">minOccurs=</span><span class="attributevalue">"1"</span>&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:text/&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/datatype&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;remarks&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;p <span class="attribute">part=</span><span class="attributevalue">"N"</span>&gt;</span>When applicable, values from the MARC relator term list (
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;ref <span class="attribute">target=</span><span class="attributevalue">"http://www.loc.gov/marc/relators/relaterm.html"</span>&gt;</span>http://www.loc.gov/marc/relators/relaterm.html<span data-indentation="4" class="element">&lt;/ref&gt;</span></div>) or code list (
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;ref <span class="attribute">target=</span><span class="attributevalue">"http://www.loc.gov/marc/relators/relacode.html"</span>&gt;</span>http://www.loc.gov/marc/relators/relacode.html<span data-indentation="4" class="element">&lt;/ref&gt;</span></div>) are recommended for
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;att <span class="attribute">scheme=</span><span class="attributevalue">"TEI"</span>&gt;</span>role<span data-indentation="4" class="element">&lt;/att&gt;</span></div>.<span data-indentation="3" class="element">&lt;/p&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/remarks&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/attDef&gt;</span></div>
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Constraints</strong></td>
         <td class="wovenodd-col2">
            <div>
               <div>@nymref attribute should have content.</div>
               <div>The value in @nymref should correspond to the @xml:id attribute of an element.</div>
            </div>
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;sch:rule <span class="attribute">context=</span><span class="attributevalue">"@nymref"</span>&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;sch:assert <span class="attribute">role=</span><span class="attributevalue">"warning"</span> <span class="attribute">test=</span><span class="attributevalue">"not(normalize-space(.) eq '')"</span>&gt;</span>@nymref attribute
                     should have content.<span data-indentation="2" class="element">&lt;/sch:assert&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;sch:assert <span class="attribute">role=</span><span class="attributevalue">"warning"</span> <span class="attribute">test=</span><span class="attributevalue">"every $i in tokenize(., '\s+') satisfies substring($i,2)=//mei:*/@xml:id"</span>&gt;</span>The
                     value in @nymref should correspond to the @xml:id attribute of an
                     element.<span data-indentation="2" class="element">&lt;/sch:assert&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/sch:rule&gt;</span></div>
            </div>
         </td>
      </tr>
   </table>
</div>
---
layout: sidebar
sidebar: s1
version: "v4"
title: "data.PLACEMENT"

---

<div class="macroSpec">
   <h3 id="data.PLACEMENT">data.PLACEMENT</h3>
   <table class="wovenodd">
      <tr>
         <td colspan="2" class="wovenodd-col2">Location information.</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Module</strong></td>
         <td class="wovenodd-col2">MEI</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Used by</strong></td>
         <td class="wovenodd-col2">
            <div class="parent"><a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/add.html">add</a>/@place, <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.annot.vis.html">att.annot.vis</a> (@place)
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Declaration</strong></td>
         <td class="wovenodd-col2">
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;content&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;alternate <span class="attribute">maxOccurs=</span><span class="attributevalue">"1"</span> <span class="attribute">minOccurs=</span><span class="attributevalue">"1"</span>&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;macroRef <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.STAFFREL.html">data.STAFFREL</a>"</span></span>/&gt;</span></div>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;macroRef <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.NONSTAFFPLACE.html">data.NONSTAFFPLACE</a>"</span></span>/&gt;</span></div>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;macroRef <span class="attribute">key=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.NMTOKEN.html">data.NMTOKEN</a>"</span></span>/&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/alternate&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/content&gt;</span></div>
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Constraints</strong></td>
         <td class="wovenodd-col2">
            <div>
               <div>Other values not permitted when 'above', 'below', 'between' or 'within' is present.</div>
            </div>
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;sch:rule <span class="attribute">context=</span><span class="attributevalue">"@place[matches(., 'above') or matches(., 'below')              or matches(., 'between')
                        or matches(., 'within')]"</span>&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;sch:assert <span class="attribute">test=</span><span class="attributevalue">"matches(normalize-space(.), '^above$') or                matches(normalize-space(.),
                           '^below$') or                matches(normalize-space(.), '^between$') or         
                           matches(normalize-space(.), '^within$')"</span>&gt;</span>Other values not permitted when 'above', 'below', 'between' or 'within' is
                     present.<span data-indentation="2" class="element">&lt;/sch:assert&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/sch:rule&gt;</span></div>
            </div>
         </td>
      </tr>
   </table>
</div>
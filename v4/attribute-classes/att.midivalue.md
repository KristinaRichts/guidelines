---
layout: sidebar
sidebar: s1
version: "v4"
title: "att.midiValue"

---

<div class="classSpec att">
   <h3 id="att.midiValue">att.midiValue</h3>
   <table class="wovenodd">
      <tr>
         <td colspan="2" class="wovenodd-col2">Attributes that record MIDI values.</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Module</strong></td>
         <td class="wovenodd-col2">MEI.midi</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Members</strong></td>
         <td class="wovenodd-col2">
            <div class="parent">
               <div><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/cc.html">cc</a> (direct member of att.midiValue)
               </div>
               <div><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/dynam.html">dynam</a><span> (via <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.dynam.ges.html">att.dynam.ges</a>)</span></div>
               <div><a class="link_odd_elementSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/hairpin.html">hairpin</a><span> (via <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.hairpin.ges.html">att.hairpin.ges</a>)</span></div>
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
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;attDef <span class="attribute">ident=</span><span class="attributevalue">"val"</span> <span class="attribute">usage=</span><span class="attributevalue">"opt"</span>&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;desc&gt;</span>MIDI number.<span data-indentation="2" class="element">&lt;/desc&gt;</span></div>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;datatype <span class="attribute">maxOccurs=</span><span class="attributevalue">"1"</span> <span class="attribute">minOccurs=</span><span class="attributevalue">"1"</span>&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:ref
                           
                           <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/data-types/data.MIDIVALUE.html">data.MIDIVALUE</a>"</span></span>
                           /&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/datatype&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/attDef&gt;</span></div>
            </div>
         </td>
      </tr>
   </table>
</div>
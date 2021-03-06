---
layout: sidebar
sidebar: s1
version: "v4"
title: "data.MIDIVALUE"

---

<div class="macroSpec">
   <h3 id="data.MIDIVALUE">data.MIDIVALUE</h3>
   <table class="wovenodd">
      <tr>
         <td colspan="2" class="wovenodd-col2">MIDI values in the following range.</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Module</strong></td>
         <td class="wovenodd-col2">MEI</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Used by</strong></td>
         <td class="wovenodd-col2">
            <div class="parent"><a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.channelized.html">att.channelized</a> (@midi.port), <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.midiInstrument.html">att.midiInstrument</a> (@midi.instrnum), <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.midiNumber.html">att.midiNumber</a> (@num), <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.midiValue.html">att.midiValue</a> (@val), <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.midiValue2.html">att.midiValue2</a> (@val2), <a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.midiVelocity.html">att.midiVelocity</a> (@vel)
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Declaration</strong></td>
         <td class="wovenodd-col2">
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;content&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;rng:data <span class="attribute">type=</span><span class="attributevalue">"nonNegativeInteger"</span>&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:param <span class="attribute">name=</span><span class="attributevalue">"maxInclusive"</span>&gt;</span>127<span data-indentation="3" class="element">&lt;/rng:param&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/rng:data&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/content&gt;</span></div>
            </div>
         </td>
      </tr>
   </table>
</div>
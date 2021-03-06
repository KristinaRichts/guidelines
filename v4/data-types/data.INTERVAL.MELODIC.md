---
layout: sidebar
sidebar: s1
version: "v4"
title: "data.INTERVAL.MELODIC"

---

<div class="macroSpec">
   <h3 id="data.INTERVAL.MELODIC">data.INTERVAL.MELODIC</h3>
   <table class="wovenodd">
      <tr>
         <td colspan="2" class="wovenodd-col2">A token indicating direction of the interval but not its precise value, an indication
            of
            diatonic interval quality and size, or a decimal value in half steps. Decimal values
            are
            permitted to accommodate micro-tuning.
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Module</strong></td>
         <td class="wovenodd-col2">MEI</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Used by</strong></td>
         <td class="wovenodd-col2">
            <div class="parent"><a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/attribute-classes/att.intervalMelodic.html">att.intervalMelodic</a> (@intm)
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Declaration</strong></td>
         <td class="wovenodd-col2">
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;content&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;rng:choice&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:data <span class="attribute">type=</span><span class="attributevalue">"decimal"</span>/&gt;</span></div>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:data <span class="attribute">type=</span><span class="attributevalue">"token"</span>&gt;</span>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:param <span class="attribute">name=</span><span class="attributevalue">"pattern"</span>&gt;</span>u|d|s|n|sh|sl<span data-indentation="4" class="element">&lt;/rng:param&gt;</span></div>
                        <span data-indentation="3" class="element">&lt;/rng:data&gt;</span></div>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:data <span class="attribute">type=</span><span class="attributevalue">"token"</span>&gt;</span>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:param <span class="attribute">name=</span><span class="attributevalue">"pattern"</span>&gt;</span>(\+|\-)?[AdMmP][0-9]+<span data-indentation="4" class="element">&lt;/rng:param&gt;</span></div>
                        <span data-indentation="3" class="element">&lt;/rng:data&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/rng:choice&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/content&gt;</span></div>
            </div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Remarks</strong></td>
         <td class="wovenodd-col2">
            <p>u = up, d = down, s = same, n = neutral/unknown, sh = same or higher (but not lower),
               sl =
               same or lower (but not higher)
            </p>
         </td>
      </tr>
   </table>
</div>
---
layout: sidebar
sidebar: s1
version: "v3"
title: "macro.availabilityPart"

---

<div class="macroSpec">
   <h3 id="macro.availabilityPart">macro.availabilityPart</h3>
   <table class="wovenodd">
      <tr>
         <td colspan="2" class="wovenodd-col2">Groups elements that may appear as part of a description of the availability of and
            access to a bibliographic item.
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Module</strong></td>
         <td class="wovenodd-col2">MEI.header</td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Used by</strong></td>
         <td class="wovenodd-col2">
            <div class="parent"><a class="link_odd_classSpec" href="{{ site.baseurl }}/{{ page.version }}/elements/availability.html">availability</a></div>
         </td>
      </tr>
      <tr>
         <td class="wovenodd-col1"><strong>Declaration</strong></td>
         <td class="wovenodd-col2">
            <div xml:space="preserve" class="pre">
               <div class="indent1 indent"><span data-indentation="1" class="element">&lt;content&gt;</span>
                  
                  <div class="indent2 indent"><span data-indentation="2" class="element">&lt;rng:zeroOrMore&gt;</span>
                     
                     <div class="indent3 indent"><span data-indentation="3" class="element">&lt;rng:choice&gt;</span>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/elements/accessRestrict.html">accessRestrict</a>"</span></span>
                              /&gt;</span></div>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/elements/distributor.html">distributor</a>"</span></span>
                              /&gt;</span></div>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/elements/price.html">price</a>"</span></span>
                              /&gt;</span></div>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/elements/sysReq.html">sysReq</a>"</span></span>
                              /&gt;</span></div>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/elements/useRestrict.html">useRestrict</a>"</span></span>
                              /&gt;</span></div>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/model-classes/model.addressLike.html">model.addressLike</a>"</span></span>
                              /&gt;</span></div>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/model-classes/model.dateLike.html">model.dateLike</a>"</span></span>
                              /&gt;</span></div>
                        
                        <div class="indent4 indent"><span data-indentation="4" class="element">&lt;rng:ref
                              
                              <span class="attribute">name=<span class="attributevalue">"<a class="link_odd" href="{{ site.baseurl }}/{{ page.version }}/model-classes/model.identifierLike.html">model.identifierLike</a>"</span></span>
                              /&gt;</span></div>
                        <span data-indentation="3" class="element">&lt;/rng:choice&gt;</span></div>
                     <span data-indentation="2" class="element">&lt;/rng:zeroOrMore&gt;</span></div>
                  <span data-indentation="1" class="element">&lt;/content&gt;</span></div>
            </div>
         </td>
      </tr>
   </table>
</div>
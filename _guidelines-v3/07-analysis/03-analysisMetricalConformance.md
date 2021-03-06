---
sectionid: analysisMetricalConformance
title: "Metrical Conformance"
version: "v3"
---



It is often helpful to record whether a given staff, layer, or measure obeys the meter
established for it. The following attributes are provided for this purpose:



{% include specDesc.html version=page.version elem="att.meterconformance" atts="att.meterconformance/metcon" %}
{% include specDesc.html version=page.version elem="att.meterconformance.bar" atts="att.meterconformance.bar/metcon" %}



When used on [staff]({{ site.baseurl }}/{{ page.version }}/elements/staff.html){:.link_odd_elementSpec} or [layer]({{ site.baseurl }}/{{ page.version }}/elements/layer.html){:.link_odd_elementSpec} elements, the
**@metcon** attribute can be used to indicate if the duration of the contained events
is equal to ("c"), less than ("i"), or greater than ("o") that predicted by the time
signature. When used on the [measure]({{ site.baseurl }}/{{ page.version }}/elements/measure.html){:.link_odd_elementSpec} element, **@metcon** takes a
boolean value, where "true" indicates conformance by all staff and layer descendants
of the
measure.

In the first example below, the layer, staff, and measure all match the prevailing
meter. In
the second example, however, the first layer does not comply with the meter, making
the staff
containing it and measure as a whole non-compliant. When there is a single layer or
when all
the layers on a staff agree with each other, metrical compliance can be indicated
on the [staff]({{ site.baseurl }}/{{ page.version }}/elements/staff.html){:.link_odd_elementSpec} element. When, however, not all layers have the same value for
**@metcon**, then it is necessary to omit **@metcon** at the staff level. The
value of **@metcon** on the measure level can usually be computed based on the values of
its layer and staff sub-elements.

{% include plainExample.html example="examples/analysis/analysis-sample177.xml" valid="true" version=page.version %}

{% include plainExample.html example="examples/analysis/analysis-sample178.xml" valid="true" version=page.version %}


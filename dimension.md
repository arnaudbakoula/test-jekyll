---
layout: "dimension"
title: Dimension
# permalink: /dimension
var_intro: "dimension/intro.md"
var_about: "dimension/about.md"
var_work: "dimension/work.md"
var_contact: "dimension/contact.md"
var_elements: "dimension/elements.md"
---

{% include_relative {{ page.var_intro    }} id="intro"%}
{% include_relative {{ page.var_about    }} id="about"%}
{% include_relative {{ page.var_work     }} id="work" %}
{% include_relative {{ page.var_contact  }} id="contact" %}
{% include_relative {{ page.var_elements }} id="elements" %}

---
layout: page
permalink: /papers/
title: papers
description: papers by language
languages: ['British Creole', 'Guinea Creole', 'Guyanese', 'Haitian', 'Mauritian', 'Naija', 'Singlish', 'West African Pidgin', ]
nav: true
---
<div class="publications">

{%- for l in page.languages %}
  <h2 class="language">{{l}}</h2>
  {% bibliography -f papers -q @*[language={{l}}]* %}
{% endfor %}

</div>

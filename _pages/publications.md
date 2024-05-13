---
layout: page
permalink: /papers/
title: Papers
description: Papers by language.
languages: ['British Creole', 'Guinea Creole', 'Guyanese', 'Haitian Kreyol', 'Mauritian Creole', 'Nigerian Pidgin', 'Singlish', 'West African Pidgin', 'Jamaican Creole English', 'Guadeloupean Creole', 'Antillean Creole', 'Krio', 'Cameroonian Pidgin', 'Seychelles Creole',
'Kituba', 'Sango', 'Kabuverdianu', '*Various', ]
nav: true
---
<div class="publications">

{%- for l in page.languages %}
  <h2 class="language">{{l}}</h2>
  {% bibliography -f papers -q @*[language={{l}}]* %}
{% endfor %}

</div>

---
layout: about
title: home
permalink: /
subtitle: 

profile:
  align: right
  image: 
  address: >

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

This page aims to centralize NLP resources for Creoles. This is an open community effort and we welcome updates via [pull requests](https://docs.github.com/es/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests) on this website's [github repository](https://github.com/creole-nlp/creole-nlp.github.io).

Below is a table summarizing resources and their availability. The resource column links to the official url, where applicable. The status column includes links that have been verified, where applicable.  
Papers on Creoles are collected [here](/papers).

<table>
<tr>
  <td> <b> Language </b> </td>
  <td> <b> Resource </b> </td>
  <td> <b> Description </b> </td>
  <td> <b> Status </b> </td>
</tr>
{% for row in site.data.table.content_hash %}
<tr>
  <td>{{row.Language}}</td>
  <td><a href="{{row.dataset_url}}">{{row.Resource}}</a> <a href="{{row.paper_url}}">{{row.paper_ref}}</a></td>
  <td>{{row.Description}}</td>
  <td><a href="{{row.dataset_url_verified}}">{{row.Status}}</a></td>
</tr>
{% endfor %}
</table>

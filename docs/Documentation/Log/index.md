---
title: log
layout: page
parent: Documentation
has_toc: false
---

# `log`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

`log` is a class providing useful utilities to deal with errors, logs and messages.

{%- assign children = site.pages | where: "parent", page.title -%}
{%- assign parts = "properties, methods" | split: ", " -%}

{% for part in parts %}
## {{ part | capitalize }}

{%- for child in children -%}
  {%- assign type = child.path | downcase | split: "/" | slice: -2 -%}
  {%- if type[0] == part %}
- [`{{ child.title }}`]({{ child.url | relative_url }})
  {%- endif -%}
{%- endfor %}
{% endfor %}

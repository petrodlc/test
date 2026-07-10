---
title: spectra
layout: page
parent: Documentation
has_toc: false
---

# `spectra`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

`spectra` is the main (and currently the only) class provided by {{ site.title }}.
It provides all the processing utilities for set of spectrums

{% assign children = site.pages | where: "parent", page.title -%}
{%- assign parts = "properties, methods" | split: ", " -%}

{%- for part in parts %}
## {{ part }}

{%- for child in children -%}
  {%- assign type = child.path | downcase | split: "/" | slice: -2 -%}
  {%- if type[0] == part %}
- [`{{ child.title }}`]({{ child.url | relative_url }})
  {%- endif -%}
{%- endfor %}
{%- endfor -%}

## Methods

{%- for child in children -%}
  {%- assign type = child.path | downcase | split: "/" | slice: -2 -%}
  {%- if type[0] == "methods" %}
- [`{{ child.title }}`]({{ child.url | relative_url }})
  {%- endif -%}
{%- endfor %}

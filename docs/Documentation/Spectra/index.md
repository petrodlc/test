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

## Properties

- [`spectra.bkg`][bkg]
- [`spectra.count`][count]
- [`spectra.data`][data]
- [`spectra.fit`][fit]
- [`spectra.mean_data`][mean data]
- [`spectra.mean_shift`][mean shift]
- [`spectra.name`][name]
- [`spectra.shift`][shift]

## Methods

## Test

{{ page.path | split:"/" | slice: -2 }}

{% for p in site.pages -%}
  {%- if page.title == p.parent -%}
  {%- assign type = p.path | split: "/" | slice: -2 -%}
- [`{{- p.title -}}`]({{- p.url | relative_url -}}) -- {{ type }}
{{ nil }}
  {%- endif -%}
{%- endfor %}

<!--------------------------------------------------------------------------->

[bkg]: {{ site.url }}/Documentation/Spectra/Properties/bkg "spectra.bkg"
[count]: {{ site.url }}/Documentation/Spectra/Properties/count "spectra.count"
[data]: {{ site.url }}/Documentation/Spectra/Properties/data "spectra.data"
[fit]: {{ site.url }}/Documentation/Spectra/Properties/fit "spectra.fit"
[mean data]: {{ site.url }}/Documentation/Spectra/Properties/mean_data "spectra.mean_data"
[mean shift]: {{ site.url }}/Documentation/Spectra/Properties/mean_shift "spectra.mean_shift"
[name]: {{ site.url }}/Documentation/Spectra/Properties/name "spectra.name"
[shift]: {{ site.url }}/Documentation/Spectra/Properties/shift "spectra.shift"

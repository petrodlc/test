---
title: spectra.fit
layout: page
parent: spectra
---

# `spectra.fit`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

The fits for each spectrums.

Two-dimensional table, storing fitted line for each spectrum, computed at call time from [`spectra.fit_params`][fit params].

- *n* represents the number of spectrums in this class instance
- *m* is the number of measure points par spectrum (should be the same for all)

### Getter

#### Returns
{: .no_toc }
- fit ([`numpy.ndarray`][ndarray]{:target="_blank"}(`numpy.float`) of shape (*m*, *n*)):\
  the computted fit lines

<!--------------------------------------------------------------------------->

[data]: {{ site.url }}/Documentation/Spectra/Properties/data "spectra.data"
[fit params]: {{ site.url }}/Documentation/Spectra/Properties/fit_params "spectra.fit_params"
[ndarray]: https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html "numpy.ndarray"

---
title: spectra.shift
layout: page
parent: spectra
---

# `spectra.shift`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

The raman shifts for all spectrums.

Two-dimensional table, storing raman shifts each spectrum, equivalent to [`spectra.data[:, 0, :]`]({{ site.url }}/Documentation/Spectra/Properties/data).

- *n* represents the number of spectrums in this class instance
- *m* is the number of measure points par spectrum (should be the same for all)

### Getter

#### Returns
{: .no_toc }
- shift ([`numpy.ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html){:target="_blank"}(`numpy.float`) of shape (*m*, *n*)):\
  a copy of the actual raman shift stored in the data property

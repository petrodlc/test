---
title: spectra.mean_data
layout: page
parent: spectra
---

# `spectra.mean_data`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

The mean data from all spectrums.

Three-dimensional table, storing data mean values (`spectra.mean_data[:, :, 0]`) and standard deviation (`spectra.mean_data[:, :, 1]`) computed along 3<sup>rd</sup> axis (spectrums).
Its value is distinct from the defaul only after [`spectra.compute_mean_data`]({{ site.url }}/Documentation/Spectra/Methods/compute_mean_data) has been called
and before [`spectra.data`]({{ site.url }}/Documentation/Spectra/Properties/data) is [set]({{ site.url }}/Documentation/Spectra/Properties/data/#Setter) to a new value.

- *n* represents the number of spectrums in this class instance
- *m* is the number of measure points par spectrum (should be the same for all)

### Getter

#### Returns
{: .no_toc }
- mean_data ([`numpy.ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html){:target="_blank"}(`numpy.float`) of shape (*m*, 2, *n*)):\
  a copy of the actual mean_data stored in the class instance

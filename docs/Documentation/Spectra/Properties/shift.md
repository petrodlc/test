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
Two-dimensional table, storing raman shifts each spectrum, equivalent of `spectra.data[:, 0, :]`.
<a href="{{ site.url }}> test </a>

- *n* represents the number of spectrums in this class instance
- *m* is the number of measure points par spectrum (should be the same for all)
- \* is any size

### Getter

#### Returns
{: .no_toc }
- data ([`numpy.ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html){:target="_blank"}(`numpy.float`) of shape (*m*, 3, *n*)):\
  a copy of the actual data stored in the class

### Setter

Raplace the old data with a copy of the data provided, and resets all other attributes except [`name`]({{ site.url }}/Documentation/Spectra/Properties/name) to their default value.

#### Parameters
{: .no_toc }
- data (array like (`float`) of shape (*, 3, *)):\
  the data to store

### Deleter

Resets to a [`numpy.ndarray`](https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html){:target="_blank"} of size (0, 3, 0) filled with `None`.
Resets all properties but [`name`]({{ site.url }}/Documentation/Spectra/Properties/name) to their default values.

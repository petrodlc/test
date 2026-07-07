---
title: spectra.data
layout: page
parent: spectra
---

# `spectra.data`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

The main data contained in the class.
Three-dimensional table, storing raman shifts and corresponding signal and background intensities for each spectrum.

- *n* represents the number of spectrums in this class instance
- *m* is the number of measure points par spectrum (should be the same for all)
- \* is any size

### Getter

#### Returns
{: .no_toc }
- data (`numpy.ndarray(numpy.float)` of shape (*m*, 3, *n*)):\
  a copy of the actual data stored in the class

### Setter

#### Parameters
{: .no_toc }
- data (`array like (float)` of shape (*, 3, *)):\
  the data to store ; will be copied ; resets all other attributes except name to their default value

### Deleter

Resets to a `numpy.ndarray` of size (0, 3, 0) filled with `None`.
Resets all properties but [`name`]({{ site.url }}/Documentation/Spectra/Properties/name) to their default values.

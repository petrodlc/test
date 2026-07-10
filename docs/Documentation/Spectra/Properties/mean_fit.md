---
title: spectra.mean_fit
layout: page
parent: spectra
math: mathjax
---

# `spectra.mean_fit`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

The mean fit from all spectrums.

One-dimensional table, storing mean fit line computed at call time from [`spectra.mean_fit_params`][mean_fit_params].
It needs [`spectra.mean_fit_params`][mean_fit_params] to be initialized.

The fit is the sum of a Cauchy (or Lorentz) distribution (for D peak) and a Breit-Wigner-Fano (BWF) distribution (for G peak), with a parameter controlling the vertical offset added :
$$
f_{LBWF}(w, p) = I_D \frac{\left(\frac{\Gamma_D}{2}\right)^2}{\left(w - w_D\right)^2 + \left(\frac{\Gamma_D}{2}\right)^2}
               + I_G \frac{\left(1 + \left(2\cdot\frac{w - w_G}{Q\Gamma_G}\right)\right)^2}{1 + \left(2\cdot\frac{w - w_G}{\Gamma_G}\right)^2}
               + y_0
$$
with $ p = \left[w_G, I_G, \Gamma_G, \frac{1}{Q}, w_D, I_D, \Gamma_D, y_0\right] $.


- *m* is the number of measure points par spectrum (should be the same for all)

### Getter

#### Returns
{: .no_toc }
- mean_count ([`numpy.ndarray`][ndarray]{:target="_blank"}(`numpy.float`) of shape (*m*, 2)):\
  a copy of the actual mean intensity stored in [`spectra.mean_data[:, 0, :]`][mean data]

<!--------------------------------------------------------------------------->

[data]: {{ site.url }}/Documentation/Spectra/Properties/data "spectra.data"
[data setter]: {{ site.url }}/Documentation/Spectra/Properties/data#setter "spectra.data setter"
[mean data]: {{ site.url }}/Documentation/Spectra/Properties/mean_data "spectra.mean_data"
[compute mean data]: {{ site.url }}/Documentation/Spectra/Methods/compute_mean_data "spectra.compute_mean_data"
[ndarray]: https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html "numpy.ndarray"

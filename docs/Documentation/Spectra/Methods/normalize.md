---
title: spectra.normalize
layout: page
parent: spectra
math: mathjax
---

# `spectra.normalize`
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

```python
spectra.normalize()
```

Normalize signal and background for each spectrum.

Compute the norm of the signal function.
The norm used is


$$
\left\|f\right\|^2 = \int_I f\left(x\right)^2 dx
$$

where $$ f $$ is the function to normalize, and $$ I $$ is the interval of normalization.

For discrete cases, it become

$$
\left\|x\right\|^2 = \sum_i x_i^2
$$

with $$ x = \left\[x_0, x_1, \dots, x_n\right] $$ and $$ \left\{x_i\right\} \in f\left(I\right) $$.

### Parameters

No parameters

### Returns

No return value

### Raises

| Exception | Cause|
| :-------- | :--- |
| `NotImplementedError` | If *b* is provided for file read mode |
| `ValueError` | If *mode* is neither *t* nor *b* |

<!--------------------------------------------------------------------------->

[data]: {{ site.url }}/Documentation/Spectra/Properties/data "spectra.data"
[name]: {{ site.url }}/Documentation/Spectra/Properties/name "spectra.name"
[path]: https://docs.python.org/3/library/pathlib.html#concrete-paths "pathlib.Path"
[read]: https://docs.python.org/3/tutorial/inputoutput.html#methods-of-file-objects "python input and output"

---
title: Usage
layout: page
nav_order: 2
---
# Usage
{: .no_toc }

<details close markdown="block">
  <summary>
    Table of Contents
  </summary>
  {: .text-delta }
- TOC
{:toc}
</details>

Since Ramaspec consists mainly on one file containing one class, all that is needed is to import that file.

## Import
If your working directory is `/path/to/my/project`, and Ramaspec is installed in `/path/to/my/project/Ramaspec`:
```python
import Ramaspec.spectra as sp
```

## Plot

No plotting utility is currently added as matplotlib.pyplot works fine as is. If you want ploting capabilities, import this library as well :
```python
import matplotlib.pyplot as plt
```
For matplotlib usage, chack its [documentation](https://matplotlib.org/stable/api/index.html).

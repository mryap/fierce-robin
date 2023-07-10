---
title: Python for Data sampling
subtitle: Using sampling to estimate descriptive statistics for a large dataset
date: 2020-03-19T14:17:12.250Z
template: post
---
Here a quick note using sampling to efficiently estimate descriptive statistics for a large data-set. 

```
subset = sample(big_data, k=250)
xbar = fmean(subset)
s = stdev(subset, xbar)
quartiles = quantiles(subset)
print(xbar, s, quartiles)
```

The imports are

```
from random import sample
from statistics import fmean, stdev, quantiles
```

Alternatively, you can use  numpy.random.choice (a, size=None, replace=True, p=None) 

Why:

* numpy has basic stat.functions build in.
* numpy is fast as it runs C code under the hood.
* numpy.random.choice allows to specify marginal probabilities.

Sampling saves time. Are your data too big? Calculate statistics on a random sample. Both approaches have their specific benefits. The only thing to avoid is mixing them up.
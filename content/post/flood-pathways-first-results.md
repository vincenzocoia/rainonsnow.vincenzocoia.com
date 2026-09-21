---
title: "Early results: as floods get rarer, rain seems to matter more"
date: "2026-09-03"
---

The title of this project asks what pathways lead to a compound rain-on-snow flood. A year in, there is something to report — though not yet something to conclude.

Rather than assume that relationships can be governed by a few parameters — maybe that runoff responds to its drivers through a linear mean with normally distributed error, or that named copula families are enough to store the dependence — I'm letting machine learning do what it does best and find the patterns itself. The model learns the whole conditional distribution: give it a rainfall and a snowmelt, and it returns a full distribution over runoff. You can then turn the question around and ask which combinations of rain and snow most likely produced an event of a given return period.

What we appear to be seeing is a shift. As the return period grows, the likeliest driver mix tilts towards rainfall and away from snowmelt. In the current model, the 200-year event sits behind roughly a 9-year rainfall falling on a thoroughly ordinary snowmelt — no record snowpack required.

I would not take that to the bank yet, and the reason is specific. The model learns from the rain and snow combinations that have actually occurred, and a 200-year runoff event by construction lives outside that range. Identifying its drivers means conditioning on combinations the model has never seen, and learning stops where the data stops. The result above comes from exactly the region where that limitation bites hardest.

Fixing it is the first task of year two: we are evaluating a copula transport approach, with vine copulas as the fallback. There are smaller caveats too — the runs are on a reduced grid using ERA5-Land reanalysis rather than Earth observation data, and none of this has been through peer review.

So: a direction worth investigating, not yet a finding. More once the model can see past its own data.

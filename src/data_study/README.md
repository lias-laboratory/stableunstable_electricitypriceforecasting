# Data Study

One of the main steps in data preprocessing is getting rid of
Outliers. Figure 5 illustrates the stable and unstable periods
of the Portuguese electricity price market. By doing an IQR
(Interquartile range) test on the whole dataset, 5422 samples
are considered outliers. Those samples are price values from
the unstable part that are very high compared to the mean
price value of the stable market. By conducting an IQR test
on both stable and unstable parts, we respectively get only 827
and 111 samples considered as outliers.
At first, we can think that the huge price spikes happening in
early 2022 are Outliers. These data points are also considered
outliers by the IQR score. But by taking a closer look at
those price spikes we actually see they are not exceptional
phenomenons, they only look like spikes because the dataset
has 45 600 samples. But in reality, those spikes are following
an exponential increase in electricity prices. Therefore we
decided to keep those values and not consider them as outliers.
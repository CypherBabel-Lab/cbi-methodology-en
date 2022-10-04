# Index Divisor

The key to index maintenance is the adjustment of the index divisor. Index maintenance (e.g. addition or deletion of constituents) should not change the index level. This is achieved by adjusting the index divisor. This section describes how the adjustment of the index divisor is made given the change in total market value of the constituents.

The equation of index level is expanded to show the constituent being removed, constituent r, separately from the constituents that will remain in the index:

$$
{Index Level}{ }_{t0}=\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{r} Q_{r}}{{Divisor}_{t0}}
$$

Note that the index level and the divisor are now labeled for the time period t-1 and, to simplify this example, that we are ignoring any possible IWF and adjustments to share counts. After stock r is replaced with stock s, the equation will read:

指数水平和指数除数的下角标现在被标记为t0。作为简化的例子，我们忽略被剔除成分以外的其它成分调整。将成分r替换为成分s后，等式如下：

$$
{Index Level}{ }_{t1}=\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{s} Q_{s}}{{Divisor}_{t1}}
$$

以上等式中，t0是剔除成分r和增加成分s之前的时刻，t1是提出成分r和增加成分s之后的时刻。按照设计要求，t0和t1时刻Index Level必须相等，所以将以上两个等式联合处理，得到：

$$
\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{r} Q_{r}}{{Divisor}_{t0}} = \frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{s} Q_{s}}{{Divisor}_{t1}}
$$

由此可知，当剔除成分r和增加成分s时，保持指数水平不变的新的除数计算方法为：

$$
{Divisor}_{t1} = {Divisor}_{t0}*\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{s} Q_{s}}{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{r} Q_{r}}
$$

# Index Divisor

The key to index maintenance is the adjustment of the index divisor. Index maintenance (e.g. addition or deletion of constituents) should not change the index level. This is achieved by adjusting the index divisor. This section describes how the adjustment of the index divisor is made given the change in total market value of the constituents.

The equation of index level is expanded to show the constituent being removed, constituent r, separately from the constituents that will remain in the index:

$$
{Index Level}{ }_{t0}=\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{r} Q_{r}}{{Divisor}_{t0}}
$$

Note that the index level and index divisor are now labeled for the time _t0_. For purpose of simplification, we are ignoring any possible events except the replacement of a constituent. After constituent _r_ is replaced with constituent _s_, the equation is:

$$
{Index Level}{ }_{t1}=\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{s} Q_{s}}{{Divisor}_{t1}}
$$

In the equations, _t0_ is the moment right before constituent _r_ is deleted from and constituent _s_ is added to the index, and _t1_ is the moment right after the event. By design, _IndexLevelt0_ is equal to _IndexLevelt1_. Combining and rearranging these two equations, the adjustment to the index divisor can be determined from the index market value before and after the change:

$$
\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{r} Q_{r}}{{Divisor}_{t0}} = \frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{s} Q_{s}}{{Divisor}_{t1}}
$$

Therefore, the new divisor after the maintenance is:

$$
{Divisor}_{t1} = {Divisor}_{t0}*\frac{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{s} Q_{s}}{\left(\sum_{i} P_{i} * Q_{i}\right)+P_{r} Q_{r}}
$$

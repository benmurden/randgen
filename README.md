randgen
=======

Node.js package for generating different kinds of random numbers: Uniform,
Normal/Gaussian, Poisson, Chi-squared, Cauchy.

Installation:
=============

    npm install randgen

Features:
=========

* Supported distributions: Uniform, Normal, Poisson, Chi-Square, Cauchy
* Vector versions of all supported distributions

Usage:
======

Generate Gaussian random numbers:

    num = rnorm();     // standard normal
    num = rnorm(2, 5); // normal with mean 2 and standard deviation of 5

Chi-Squared:

    num = rchisq(4);   // 4 degrees of freedom

Random element from a list:

    num = rlist([1, 2, 3, 4]);

Others: `runif`, `rpoisson`, `rcauchy`, `rbernoulli`

You can also generate vectors of random numbers:

    nums = rvnorm(100); // generate 100 standard normal values

Others: `rvunif`, `rvchisq`, `rvpoisson`, `rvcauchy`, `rvlist`, `rvbernoulli`

It also includes a handy `histogram()` function to convert an array of numbers
into a set of bins:

    bins = histogram(data);     // defaults to 10 bins
    bins = histogram(data, 20); // 20 bins

LICENSE:
========

MIT License

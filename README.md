# Optimizing-ARIMA-for-SystemML

The Autoregressive Integrated Moving Average (ARIMA) model is one of most broadly
used time series models and applied to better understand and forecast time series data.
As a generalization of the Autoregressive Moving Average (ARMA) model, which itself is a
combination of the Autoregression and MA model, it can also be used to analyze time
series that are non-stationary.

The goal of this research project was to complete the implementation of the ARIMA
algorithm for SystemML using the Declarative Machine Learning Language.

This report starts of with a short introduction that gives an example for the applications of
large scale time series analysis to demonstrate its importance and then discusses the focus
and motivation of the project in more detail. In the second chapter, the ARIMA model is
explained and discussed in full with a focus on the systems of linear equations which
is at the center of the model. An important part of the algorithm is to find a solution
for these linear systems, which is why there is a completely separate section in the second
chapter that discusses different approaches used for solving linear systems and particular
the linear systems produced by ARIMA models, which have some key characteristics that
can be exploited to find a solution more effienctly. To give some more background on the
over all training algorithm a number of optimization methods commonly used are outlined
and discussed. The third chapter then explains why and which solvers for the system of
linear equations were chosen and discusses the implementation of ARIMA in DML. It is
also describing how exactly the performance and precision of the script will be measured
and how it is tested for correctness. Afterwards, the results are presented and finally the
methodology as well as the results are discussed and assessed.
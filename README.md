# Forward Starting Option

A model is presented for pricing European exercise, forward starting options on an underlying equity.

Let St denote the spot equity price at time t. We assume that the process satisfies under the domestic risk-neutral probability measure, a stochastic differential equity (SDE) of the form. This difficulty can be avoided by approximating the SDE dynamics via a partial differential equation (PDE).

 
Note that the volatility depends only on time and on the instantaneous value of the state variable S, but does not explicitly depend on Wt.In practice, option price or implied volatility surfaces are available at points on a relatively sparse grid of strike and tenor pairs. Using analytical expressions to determine the local volatility function then likely yields inaccurate results due to the numerical instability from calculating first, and especially, second derivatives.

Volatility surface input can be specified according to the following three respective representations:

	Skew-tail parametric model (i.e., the surface is fully specified by three parameters, which are respectively called “skew”, “tail”, and “anchor”),
	Polynomial parametric model (i.e., specified by coefficients of polynomial in strike and 1/√tenor and
	Implied volatility grid.

The valuation requires two interest rate curve inputs. One curve, called the “hedge curve”, is specified by a list of n term and continuously compounded zero rate pairs and is intended for use in computing forward equity values.

The other, called the “discount curve, is specified by a list of m term and continuously compounded zero rate pairs, and is intended for use in calculating discount factors,

References:

https://finpricing.com/lib/EqBarrier.html

https://osf.io/37fbt/download

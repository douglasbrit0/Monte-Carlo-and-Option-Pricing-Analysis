**Monte Carlo and Option Pricing**

This project implements and analyzes numerical techniques for pricing European and binary (cash-or-nothing) call options under the Black–Scholes model. It was developed as part of a Quantitative Finance course exam.

**Overview**

We estimate the value of an option at time t using the risk-neutral expectation:

```r
V(S_t, t) = exp(-r(T - t)) * E_Q[Payoff(S_T)]
```
We compare the following methods:

Closed-form Black–Scholes formulas for:

* European call options

* Binary (cash-or-nothing) call options

* Euler–Maruyama discretization of the SDE

* Milstein scheme (captures the Itô correction)

**Key Features**

Monte Carlo simulations to estimate option prices

 * Convergence analysis:

   * Vary number of simulation paths N

   * Vary number of time steps M

 * Error vs. 1/sqrt(N) convergence plots

 * Histogram of binary payoffs to show bimodal variance

* Parameter sensitivity analysis

* Comparison to closed-form prices

**Technologies Used**

Python (NumPy, Matplotlib)

Jupyter Notebook

**Getting Started**
```bash
git clone https://github.com/your-username/monte-carlo-option-pricing.git
cd monte-carlo-option-pricing
jupyter notebook Monte-Carlo-and-Option-Pricing.ipynb
```

**License**
MIT License.

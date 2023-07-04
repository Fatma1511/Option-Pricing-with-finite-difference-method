# Option-Pricing-with-finite-difference-method
The purpose of this project is to compute the price and greeks of a vanilla option
with european or american exercise. The Black–Scholes partial differential equation
will be solved using a numerical method. The PDE solver is written in C++.
The user interface will use Excel.
## Inputs
1. The contract type : call or put.
2. The exercise type : european or american.
3. The option maturity.
4. The option strike.
5. The computation date. The default value is today.
6. The time mesh parameters.
7. The spot mesh parameters.
8. The current price of the underlying (spot) S0.
9. The risk free interest rate. A constant value, positive or negative will be used.
10. The volatility σ.
## Computation method
A finite difference discretization with the Theta method will be used.
## Validation
In order to validate the results we will use the Black–Scholes formula to compare the numerical method with the explicit solution. You will also verify that the code verifies the equivalence between american and european exercises for calls with r > 0 and for puts with r < 0.
## Outputs:
Let P (S, t, r, σ) be the price of the option. The code must compute the following outputs :
1. The option theoretical price : P .
2. The option ∆ : ∂P/∂S .
3. The option Γ : ∂2P/∂S2 .
4. The option Θ : ∂P/∂t .
5. The option ρ : ∂P/∂r .
6. The option vega : ∂P/∂σ .
7. A graph of the option price P (S, T0) as a function of the underling share price (S) at the valuation date T0.
8. A graph of the option ∆(S, T0) as a function of the underlying share price (S) at valuation date T0.
9. A graph of the exercise boundary of an américain option at a given date.

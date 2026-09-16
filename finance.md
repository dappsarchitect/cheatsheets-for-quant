# Notes for Finance 

## When we say we want to "price the option", is this price nothing but just the premium that the buyer pays the seller when they enter into the option contract?

Yes, the price is the premium. Also...

## What are the different styles of options?

Quick answer: European options, American options, Bermudan options and Asian options.

- European options: can only be exercised on the exact day of expiration $T$.
- American options: can be exercised at any time on or before the expiration date $T$. This feature adds significant value (especially for options on dividend-paying stocks) and makes them harder to price mathematically.
- Bermudan options: can be exercised only on specific, pre-determined dates prior to expiration, e.g., the first day of every month.
- Asian options: the payoff depends on the average price of the underlying asset over a specified period, rather than the price on the exact expiration date.

## What are call options and put options?

- Call option: Gives the holder the right (but not the obligation) to **buy** the underlying asset at a fixed price (strike price $K$) on or before expiration $T$; becomes profit if the asset price **goes above** strike price $K$.

- Put option: Gives the holder the right (but not the obligation) to **sell** the underlying asset at a fixed price (strike price $K$) on or before expiration $T$; becomes profit if the asset price **drops below** strike price $K$.

## Definition of Volatility $\sigma$

$$d(ln S_t) = (\mu-\frac{1}{2}\sigma^2)dt+\sigma dW_t$$

where $S_t$ is the stock price at time $t$, and $\sigma$ is the annualized standard deviation of the stock's log-returns, and scales the randomness driven by standard Brownian motion (Wiener process) $dW_t$.

## Table of Definitions

| Acronyms | Full Expressions | Explanations |
|--- |--- |--- |
| IBOR | Interbank Offered Rate | Examples include LIBOR, TIBOR, EURIBOR; the historical reference rates representing the average interest rate at which major global banks were willing to lend unsecured funds to each other in the interbank market. Following manipulation scandals and declining interbank lending volume, regulators globally phased out IBORs in favour of transaction-based Risk-free Rates. |
| RFRs | Risk-free Rates | See above. |
| LIBOR | London Interbank Offered Rate | The long-time dominant benchmark for global interest rate contracts (e.g. USD, GBP, JPY, EUR, CHF). It was term-based (e.g. 1-month, 3-month, 6-month LIBOR). Currently effectively fully discontinued globally. Legacy LIBOR models have been replaced by OIS/RFR frameworks. |
| TONA | Tokyo OverNight Average (rate) | The overnight risk-free benchmark for JPY, calculated by the Bank of Japan based on actual uncollateralised overnight money market transactions. |
| SOFR | Secured Overnight Financing Rate | The overnight risk-free benchmark for USD, backed by Treasury repurchase agreement (repo) transactions. |
| ESTR | Euro Short-Term Rate | The overnight risk-free benchmark for EUR, calculated by the European Central Bank. |
| OIS | Overnight Index Swap | An interest rate swap where one counterparty pays a fixed interest rate and receives a floating rate tied to the daily compounded overnight rate such as TONA for JPY or SOFR for USD. OIS quotes form the gold-standard discount curve across all modern trading desks, replacing legacy LIBOR curves. |
| YCC | Yield Curve Control | An unconventional monetary policy tool used prominently by the Bank of Japan where the central bank targets a specific yield on long-term government bonds (specifically 10-year JGBs) by buying unlimited amounts of bonds whenever yields exceed the target threshold. YCC artificial pegs caused volatility to collapse at the 10-year point of the JPY curve and created severe distortion or discontinuities in yield curve fitting and SABR calibration. It is a classic edge case for model validation teams. |
| IRS | Interest Rate Swaps | A bilateral contract where two parties exchange interest payment streams based on a specific principal amount (notional). Typically, Party A pays a fixed rate (e.g. 0.95%) and received a floating rate (e.g. TONA), while party B does the opposite. |
| SABR | Stochastic Alpha, Beta, Rho | A mathematical model created by Hagan et al. (2002) that models the forward rate $F_t$ and its volatility $\sigma_t$ as two coupled stochastic differential equationis. It is the universal sell-side benchmark for interpolating and calibrating the swaption volatility smile. |
| FRTB | Fundamental Review of the Trading Book | It is part of the global Basel III post-crisis reforms, often referred to industry-wide as Basel IV endgame. It is the comprehensive set of global bank regulatory capital rules governing market risk in trading books. Two main components for model validation include: replacing Value-at-Risk (VaR) with Expected Shortfall (ES) at a 97.5% confidence level to capture tail risk during market shocks, and imposing strict Profit and Loss Attribution (PLA) testing so requiring banks to prove their risk-management pricing models align tightly with daily front-office P&L, the failure of which forces a bank onto expensive standardised regulatory capital penalties. |

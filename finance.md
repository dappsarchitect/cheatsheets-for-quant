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

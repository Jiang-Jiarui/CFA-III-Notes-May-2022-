# CH4 Part1: Derivatives

[toc]

## Option Management

### Option Fundamentals

#### Moneyness

Comparing current price with the strike price, **Moneyness** describes the value of an immediate exercise of an option

- In the money: positive payoff
- At the money: zero payoff
- Out of the money: negative payoff

#### Intrinsic value and time value

When it comes to options,  **value** and **payoff** are the amount excluding the options premium, **profit** and **Gain/Loss** are the amount including options premium

- Intrinsic value: the amount of immediate exercise
- Time value: option premium - intrinsic value

#### Factors affecting the value of an option

|           Factor           | Calls | Puts |
| :------------------------: | :---: | :--: |
|      Underlying price      |   +   |  +   |
|        Strike price        |   -   |  +   |
|         Volatility         |   +   |  +   |
|       Risk-free rate       |   +   |  -   |
|     Time to expiration     |   +   |  +   |
| Payments on the underlying |   -   |  +   |
|       Carrying cost        |   +   |  -   |

\* + is positively related, - is negatively related

- There is an exception to the general rule that European put option thetas are negative. The put value may increases as the option approaches maturity if the option is deep in-the-money and close to maturity

#### The BSM model to value an option

$$C_0=[S_0\times N(d_1)]-[X\times e^{-R_f^c\times T}\times N(d_2)]
$$

#### Historical Volatility and Implied Volatility

- **Historical volatility** is using historical data to calculate the variance and standard deviation of the continuously compounded returns
- **Implied volatility** is using current market price and BSM to work backwards to get the volatility

### Synthetic Asset

- **Put call parity**

$$ C+Ke^{-rT} = P+S
$$

- **Synthetic long/short forward**
  - Long call + short put = long forward
- **Synthetic call/put**
  - long call = long asset + long put
  - long put = short asset + logn call

### Option Strategies

#### Covered call

- Hold the underlying asset and sell a call option on the same underlying asset
- Purpose
  - Yield enhancement
  - Reducing a position at a favorable price (ITM call option)
  - Target price realization
![covered call](Asset/1.%20Covered%20Call.png)

#### Protective put

- Hold the underlying asset and buy a put on the same underlying asset
- Protective put is used to limit the downside at the cost of the put premium

![protective put](Asset/2.%20protective%20put.png)

- Both covered call and protective put are not delta neutral
- Cash secured put
  - writes a put option, and deposits an amount of money equal to the exercise price

#### Collar

- components
  - hold the underlying stock
  - buy a put with K lower than S
  - sell a call with K higher than S
- The cost of the put is largely and often precisely offset by the income from writing the call
- A collar limit the downside risk at a cost of giving up the upside return

![Collar](Asset/3.%20Collar.png)

#### Bull spread

- component
  - buying one call
  - sell another call with a higher K
- The buyer of a bull spread using call expects the stock price to rise and the purchased call to finish in-the-money. However, the buyer does not believe that the price of the stock will rise above the exercise price for the out-of-the-money written call
- A bull spread limit the downside risk at a cost of giving up the upside return
![bull spread](Asset/4.%20bull%20spread.png)

#### Bear spread

- With a bear spread, you buy the higher exercise price and write the lower exercise price
- component
  - buy one call
  - sell another call with a lower K

![bear spread](Asset/5.%20bear%20spread.png)

#### Straddle

- A long straddle is creadted by purchasing a call and a put with the same strike price and expiration
  - This strategy bets on higher volatility
- A short straddle is creadted by selling a call and a put with the same strike price and expiration
  - This strategy bets on lower volatility

![Straddle](Asset/6.%20Straddle.png)

#### Calendar Spread

- Sell a near-dated call and buy a longer-dated call
- same underlying asset and same strike price
- Taking advantage of time decay is a primary motivation behind a calendar spread

#### Summary: option strategies selection

![summary](Asset/7.%20summary.png)

### Option Greeks

![option greeks](Asset/8.%20option%20greeks.png)

#### Delta

- delta = Change in option price / Change in underlying price
- $delta_{call} = \Delta C/ \Delta S$
- $delta_{call} = \Delta P/ \Delta S =delta_{call} - 1$
- BSM perspective
  - the call option's delta is equal to N(d~1~) from the BSM model, and the put option's delta equals N(d~1~)-1
- The call delta increases from 0 to 1 as stock price increases
- The put delta increases from -1 to 0 as stock price increases
- Then t approaches maturity, a in-the-money call's delta is close to 1, while a out of the money call's delta is close to 0

![call option delta](Asset/9.%20call%20option%20delta.png)

- Delta hedge
$$ number\;of\;options\;needed\;to\;delta\;hedge = \frac{number\;of\;shares\;hedged}{delta\;of\;call\;option}
$$

#### Gamma

- gamma = Change in option delta / Change in underlying price
- $gamma = \Delta delta/ \Delta S$
- Call and put options on the same stock with the same T and X have equal gammas
- If the option is deep in- or out-of-the-money, gamma approaches zero
- **Gamma is largest when the option is near the money**, which means delta is very sensitive to a change in the stock price

### Volatility Smile

- Volatility smile is a plot of the implied volatility of an option as a function of its strike price
- The implied volatility of a European call option is always the same as the implied volatility of a European put option when the two have the same strike price and maturity date
- The implied volatility is relatively low for at-the-money options. It becomes progressively higher as an option moves either into the money or out of the money
- Volatility smile for currency options
![volatility smile for currency options](Asset/10.%20volatility%20smile%20for%20currency%20options.png)
- Volatility skew for equity options
![Volatility skew for equity options](Asset/11.%20Volatility%20skew%20for%20equity%20options.png)
  - reasons for smile skew in equity options
    - **Leverage**: As a company's equity declines in value, the company's leverage increases. This means that the equity becomes more risky and its volatility increases
    - **Volatility feedback effect**: As volatility increases (decreases) because of external factors, investors require a higher (lower) return and as a result the stock price declines (increases).
    - Crashophobia
- Risk reversal
  - long call and short put on the same underlying with same expiration
- Alternative ways of characterizing the volatility smile
  - The volatility smile is often calculated as the relationship between the implied volatility and **K/S~0~** rather than as the relationship between the implied volatility and K
  - A refinement of this is to calculate the volatility smile as the relationship between the implied volatility and **K/F~0~**, where F~0~ is the forward pirce of the asset for a contract maturing at the same time as the options that are considered
- Another approach to defining the volatility smile is as the relationship between the implied volatility and the **delta** of the option
- Volatility surfaces combine volatility smiles with the time to maturity and K/S~0~
  - Implied volatility tends to be an increasing (decreasing) function of maturity when short-dated volatilities are historically low (high)

![volatility surface](Asset/12.%20Volatility%20Surface.png)

## Swaps, Forwards, and Futures Strategies

### Managing Interest rate risk

#### Interest rate swap

- A **payer swap** is a contract to make a series of **fixed-rate payments** and receive a series of floating-rate payments, both based on a specified notional principal (amount).
- Interest rate swaps can be used to:
  - convert between floating exposure and fixed exposure
  - alter the duration of a fixed-income portfolio

![Converting Fixed-Rate and Floating-Rate Exposures](Asset/13.%20Converting%20Fixed-Rate%20and%20Floating-Rate%20Exposures.png)

- Duration of a swap
  - A pay-fixed, receive-floating swap has a negative duration, because the duration of fixed-rate bond is positive and larger than the duration of a floating-rate bond, which is near zero
  - A pay-floating, receive-fixed swap has a positive duration
  - $$Duration_{pay-floating}=Duration_{fix}-Duration_{floating}>0
  $$
  - For floating-rate side, it doesn't has zero duration at all time, especially when the cash flow has been set. The duration of floating-rate side will be the time to next payment if the payment is known
    - eg. for a semi-annually reset swap, the duration of the floating payment is 0.5 on any coupon reset days

- Market value risk and cash flow risk
  - Market value risk is a concern with fixed-rate instruments
  - Cash flow risk, uncertainty regarding the size of cash flows, is a concern with floating-rate instruments
  - there is a tradeoff between market value risk and cash flow risk

- Use IRS to modify the portfolio duration
$$NP_s=MV_p(\frac{MD_T-MD_p}{MD_s})
$$

#### Forward Rate Agreements (FRAs)

- FRAs are typically used to hedge the uncertainty about a future short-term borrowing or lending rate
- The long position in an FRA will receive a payment at settlement if the market rate of interest rate is higher than the (forward) rate specified in the FRA, and will make a payment to settle the FRA otherwise
- FRA payment is made at the future borrowing or lending date(or FRA expiration date) and is equal to
  - the present value of the difference in interest between a market-rate loan and a loan at the forward rate (rate specified in the FRA)
  - ![FRA](Asset/14.%20FRA.png)

#### Short-dated interest rate (STIR futures): Eurodollar futures

- STIR futures are conceptually very similar to FRAs. The standardization of futures means that contracts are only available on specific maturities (typically quarterly)
- Characteristics of Eurodollar futures
  - Notional principal: $1 million
  - Quoted price: 100-annualized forward rate
    - The pricing convention means that futures prices will rise when forward rates fall
    - The forward interest rate is calculated from current spot LIBOR rates in the same way the forward price of an FRA is established
  - Contract period: 3-month
  - One basis point change in the forward rate will cause the contract's value to change by \$25 (1 million $\times$ 0.01% $\times$ 90/360 = 25)
- Differences between Eurodollar futures and FRA
  - A long Eurodollar futures position will increase in value as forward rates decreases, and decrease in value as forward rates increase
  - A long FRA position, which increases in value as forward rates increase, and decreases in value as forward rates decrease
- Similarity between Eurodollar futures and FRA
  - Both Eurodollar futures and FRA agreements allow lenders and borrowers to lock in rates for future borrowing and lending

#### Longer-dated fixed-income futures: T-bond futures

- STIR futures can be used to hedge the interest rate risk of short-maturity bonds, however, **liquidity of interest rate futures decreases for forward rates further in the future**
- Longer-maturity bonds are most often hedged with fixed-income futures (bond futures), which have very good liquidity
  - **Treasury futures** are widely used as fixed-income futures, which are available on T-bills, Treasury notes and Treasury bonds and are traded on the CBOT (Chicago Board of Trade) and CME (Chicago Mercantile Exchange) in US
- Characteristics of T-bond Futures
  - **Underlying**: Hypothetical 30 year treasury bond with 6% coupon rate
  - **Bond can be deliverable**: $100,000 par value T-bonds with any coupon but with a maturity of at least 15 years.(US regulation)
  - **Settlement**: Physical delivering
  - **Notional principl**e: 0.1M
  - **Quotes** are in points and 32nds: A price quote of 95-18 is equal to 95.5625 and a dollar quote of $95,562.50
  - The short has a delivery option to choose which bond to deliver
  - Each bond is given a **conversion factor (CF)**, which means a specific bond is equivalent to CF standard bond underlying in futures contract
    - For a specific Bond A: $ FP_A = FP_f \times CF_A $
  - The target dollar duration of portfolio is set equal to the dollar duration of the bonds we hold and the dollar duration of the futures contracts
    - $$ BPV_T=BPV_P+BPV_f \times BPVHR $$
    - $$ BPV_f = BPV_{CTD}\times \frac{1}{CF_{CTD}} $$
    - $$ BPVHR = \frac{BPV_T-BPV_p}{BPV_{CTD}} \times CF_{CTD} $$
    - $$ BPVHR = \frac{MD_T-MD_p}{MD_{CTD}} \times CF_{CTD} \times \frac{nominal_P}{nominal_{CTD}} $$

### Managing equity risk

#### Equity Swap

- Equity swaps can be used to create a synthetic exposure to physical stocks, allowing market participants to change their exposure to equity returns
- Equity swaps enable users to achieve the economic benefits of share ownership without the cost and expense of ownership
- Three types of equity swap
  - pay fixed rate and receive equity return
  - pay floating rate and receive equity return
  - pay one equity return and receive another equity return
- The equity return may include dividend return plus price return based on
  - A single stock
  - A basket of equities
  - An equity index

#### Equity futures and forwards

- Equity futures are exchange traded, standardized, require margin, have low transaction costs, and are available on indexes and single stocks
- Index futures have a multiplier. The actual futures price is the quoted futures price (in points) × the multiplier

| Stock Index Futures | Multipliers |
| :-----------------: | :---------: |
|    S&P 500 Index    |     250     |
|     NASDAQ 100      |     100     |
|     DJIA Index      |     10      |

- Equity forwards provide many of the same advantages but lack liquidity and but are not subject to mark-to-market margin adjustments
  - Because there is no clearinghouse, the credit quality of the counterparties is a concern.
  - The major advantage of forward contracts is they can be customized

- Equity futures can be used to alter portfolio beta
$$ N_f=(\frac{\beta_T-\beta_p}{\beta_f})(\frac{MV_p}{F})=(\frac{\beta_T-\beta_p}{\beta_f})(\frac{MV_p}{f\times multiplier})
$$

- **Cash equitization** (Cash securitization or cash overlay) refers to purchasing index futures to replicate the returns that would have been earned by investing the cash in an index with risk and return characteristics similar to those of the portfolio

### Using derivative to alter asset allocation

Altering asset allocation between equity and debt with futures

- Step1: Calculate the reallocating amount
- Step 2: To reallocate an amount from equity to bonds:
  - Remove all systematic risk from the position (beta = 0) by shorting equity futures
  - Add duration to the position (BPV > 0) by going long bond futures
- Step 3: To reallocate an amount from bonds to equity:
  - Remove all duration from the position (BVP = 0) by shorting bond futures
  - Add systematic risk to the position (beta > 0) by going long equity futures

### Managing Currency risk

#### Currency Swap

- Reasons for currency swap
  - Converting a loan in one currency into a loan in another currency
    - A **cross-currency basis swap** is used in the case with ==principals switched at the beginning of the swap==
    - Cross-currency basis represents the additional cost of borrowing dollars synthetically with a currency swap relative to the cost of borrowing directly in the USD cash market
    - The additional cost indicated the foreign currency to be exhibiting negative basis. Most currencies shown a negative basis against the dollar since the financial crisis
  - Converting foreign cash receipts into domestic currency
  - Also known as **synthetic borrowing** with ==no principal switched at the beginning of the swap==
- Features of cross-currency basis swap:
  - Two notional principals exists in the currency swap and it needs to exchange and return the principal at the effective date and maturity date
  - The periodical interest cannot be netted as there are different currencies
- Features of synthetic borrowing:
  - Do not require an exchange of notional principals
  - A series of exchange-rate cash flows in the future at a fixed exchange rate
  - The amounts exchanged are based on the exchange rate and interest rate

#### Currency Forwards and Futures

Currency forwards and futures allow users to exchange a specified amount of one currency for a specified amount of another currency on a future date

$$ HR= \frac{Amount\;of\;currency\;to\;be\;exchanged}{Futures\;contract\;size}
$$

### Managing Volatility risk

#### Volatility derivatives

- The VIX Index measures implied volatility in the S&P 500 Index over a forward period of 30 days.
  - More specific, VIX computes a weighted average of implied volatility inferred from S&P 500 traded options (calls and puts) with an average expiration of 30 days.
  - Specifically, the VIX Index value is the annualized standard deviation of the expected percentage moves in the S&P 500 Index over the following 30 days.
- Vix futures
  - An equity holding can be protected from extreme downturns (tail risk) by buying VIX futures
  - Selling VIX futures creates a short volatility position and captures the volatility risk premium embedded in S&P 500 options
- Vix options
  - VIX options are cash-settled European-style options
  - VIX call options will gain in value if expectations of volatility at maturity of the option increase

#### Variance swap

- Variance swaps payoffs are based on variance rather than volatility
- In a variance swap, the buyer of the contract will pay the difference between the **fixed variance strike** agreed on in the contract and the **realized variance** (annualized) on the underlying over the period specified and applied to a variance notional
- The fixed payment is typically based on implied volatility2 (implied variance) over the period and is known at the initiation of the swap, this is referred to as the variance strike
- The variable payment is unknown at swap initiation and is only known at swap maturity. It is the actual variance of the underlying asset over the life of the swap and is referred to as realized variance
- The features of variance swap
  - no exchange of notional principal and no interim settlement periods
  - With a variance swap, there is a single payment at the expiration of the swap based on the difference between actual and implied variance over the life of the swap

$$ variance\;notional=\frac{vega\;notional}{2K}
$$

$$ settlement\;amount\;(long) = variance\;notional \times (\sigma^2-K^2)
$$

$$ settlement\;amount\;(long) = vega\;notional \times (\frac{\sigma^2-K^2}{2K})
$$

- **vega notional** represents the average profit and loss of the variance swap for a 1% change in volatility from the strike
- The Mark-to-Market value of variance swap
  - The mark-to-market valuation of a variance swap at time t will depend on realized volatility from the swap’s initiation to t, and implied volatility at t over the remaining life of the swap (T − t)
  - **step 1**:Compute expected variance at maturity (the time-weighted average of realized variance and implied variance over the remainder of the swap's life)
  - $$Expected \;variance \;to \;maturity = (\sigma^2_t\times \frac{t}{T}+(K^2_{T-t}\times \frac{T-t}{T}))$$
  - **step 2**: Compute expected payoff at swap maturity:
  - $$ Expected\;payoff = variance\;notional\times (expected\;variance\;to\;maturity-original\;strike)$$

- The Payoff of a Variance Swap Is **Convex** in Volatility
![variance swap payoff](Asset/15.%20variance%20swap%20payoff.png)

### Inferring Market Expectation

|                 Application                  |       Derivative        |
| :------------------------------------------: | :---------------------: |
|     Inferring expectations of FOMC moves     |    Fed funds futures    |
|     Inferring expectations of inflation      |        CPI swaps        |
| Inferring expectations of futures volatility | VIX futures and options |

#### Fed funds futures

- Fed funds futures contract price = 100 - Expected FFE rate
- Market participants can use Fed funds futures to infer the expected probabilities of upcoming Fed interest rate changes. Some terms and definitions used in the analysis include
  - **Federal funds rate**. This is the interest rate that deposit institutions (banks and credit unions) charge other deposit institutions for loans in the overnight interbank markets
    - The **federal funds effective (FFE) rate** is the weighted average of interest rates charged on overnight interbank loans
  - **Federal funds target rate**. This is the rate set by governors of the Federal Reserve in Federal Open Market Committee (FOMC) meetings
    - The target rate is typically set as a range (e.g. 2.25% - 2.50%).

#### Eurodollar futures

- The futures pries quote is 100 minus the futures interest rate

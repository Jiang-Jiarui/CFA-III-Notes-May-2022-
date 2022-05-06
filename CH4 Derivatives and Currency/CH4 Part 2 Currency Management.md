# CH4 Part2: Currency Management

[toc]

## Currency quotes, Currency Markets and Products

### Price and Base Currencies

- **Base currency:** with respect to a foreign exchange quotation of the price of one unit if a currency, the currency referred to in "one unit of a currency"
- **Quoting conventions:**
  - Currency pairs involving the EUR will use the EUR as the base currency (for example, GBP/EUR)
  - Currency pairs involving the GBP, other than those involving the EUR, will use the GBP as the base currency (for example, CHF/GBP)
  - Currency pairs involving either the AUD or NZD, other than those involving either the EUR or GBP, will use these currencies as the base currency (for example, USD/AUD and NZD/AUD). The market convention between these two currencies is for a NZD/AUD quote.
  - All other currency quotes involving the USD will use USD as the base currency (for example, MXN/USD).

### Bid/Asked Rule

- Bid/Asked rules
  - The bid (offer) price is the price, defined in terms of the price currency, at which the counterparty providing a two-sided price quote is willing to buy (sell) one unit of the base currency
    - E.g., quote a two-sided price on the spot USD/EUR exchange rate of 1.3648/1.3652. This quote means that the dealer is willing to pay USD1.3648 to buy one euro (bid) and that the dealer will sell one euro (offer) for USD1.3652.
  - The market width, usually referred to as dealer's spread or the bid-offer spread, is the difference between the bid and the offer
- Spot and Forward Bid/Asked Quotes
  - For illustration purposes, assume that the bid offer for the spot and forward points for the USD/EUR exchange rate are as shown in Exhibit below
  - To convert any of these quoted forward points into a forward rate, one would divide the number of points by 10,000 and then add the result to the spot exchange rate quote.

|    Maturity    | Spot Rate or Forward Points |
| :------------: | :-------------------------: |
| Spot (USD/EUR) |        1.3549/1.3651        |
|   One month    |         -5.6/ - 5.1         |
|  Three months  |        -15.9/ -15.3         |
|   Six months   |        -37.0/ -36.3         |
| Twelve months  |        -94.3/ -91.8         |

### Offsetting Transactions and Mark To Market

- Forward contracts
  - Although there is no cash flow on a forward contract until settlement date, it is often useful to do a mark-to-market valuation on a forward position before then to
    - judge the effectiveness of a hedge based on forward contracts
    - measure the profitability of speculative currency positions at points before contract maturity
  - The mark-to-market value of forward contracts reflects the profit (or loss) that would be realized from closing out the position at current market prices

### Mark-to-market Value

- Mark-to-market value of a forward contract
  - The value of a forward currency contract prior to expiration (time t) is also known as the mark-to-market value
  $$ V_t=\frac{(FP_t-FP)(contract\;size)}{(1+R(\frac{days}{360}))}
  $$

### FX Swap

FX swaps are distinct from currency swaps:

- Similar to currency swaps, FX swaps involve an exchange of principal amounts in different currencies at swap initiation that is reversed at swap maturity
- Unlike currency swaps, FX swaps have no interim interest payments and are nearly always of much shorter term than currency swaps
  - FX swaps are important for managing currency risk because they are used to "roll" forward contracts forward as they mature

### Currency options

- Currency options
  - vanilla call and put options
  - exotic options

## Effect of Currency on Portfolio Return and Risk

- Some definitions:
  - **Domestic currency** or **home currency**:The currency of the investor, i.e. the currency in which he or she typically makes consumption purchases
  - **Domestic Asset**: an asset that trades in the investor's domestic currency
  - **Foreign currency**: Currency that is not the currency in which an investor makes consumption purchases, e.g., the US dollar from the perspective of a Swiss investor
  - **Foreign assets**: asset denominated in currencies other than investor's home currency
  - **Foreign currency return (R~FC~)**: The return of the foreign asset measured in foreign-currency terms
  - **Local currency return (R~FX~)**: The percentage change of the foreign currency against the domestic currency
  - **Domestic currency return (R~FX~)**: A rate of return stated in domestic currency terms from the perspective of the investor
    - reflects both the **foreign-currency return on an asset** as well as **percentage movement in the spot exchange rate** between the domestic and foreign currencies.
- Domestic-currency return on a portfolio of multiple
foreign assets

$$ R_{DC}= \sum_{i=1}^{n} w_i(1+R_{FC,i})(1+R_{FX,i})-1 $$

- Variance of domestic-currency return for a two asset portfolio
$$ \sigma^2(R_{DC})\approx \sigma^2(R_{FC})+\sigma^2(R_{FX})+2\sigma(R_{FC})\sigma(R_{FX}) \rho(R_{FC},R_{FX})$$

## Strategic Currency Management

- One camp of thought holds that in the long run currency effects cancel out to zero due to: **no hedge required**
- Another camp of thought notes that currency movements can have a dramatic impact on short-run returns and return volatility: hedge in the short term, no hedge in the long term

### The investment Policy Statement (IPS)

- The Investment Policy Statement (IPS) mandates the degree of discretionary currency management that will be allowed in the portfolio, how it will be benchmarked, and the limits on the type of trading polices and tools (e.g., such as leverage) than can be used
- The currency risk management policy will usually address such issues as the :
  - target proportion of currency exposure to be passively hedged
  - latitude for active currency management around this target
  - frequency of hedge rebalancing
  - currency hedge performance benchmark to be used
  - hedging tools permitted (types of forward and option contracts, etc.)

### Choice of Currency Exposure

- Diversification Considerations
- Cost Considerations

### Choice of Currency Management Strategies

- Passive hedging
  - Passive hedging is a rules-based approach that removes almost all discretion from the portfolio manager
- Discretionary hedging
  - This discretion allows the portfolio manager at least some limited ability to express directional opinions
- Active currency management
  - The portfolio manager is allowed to express directional opinions on exchange rates, but is nonetheless kept within mandated risk limits
  - The active currency manager is supposed to take currency risks and manage them for profit
- Currency overlay
  - allows the externally hired currency overlay manager to take directional views on future currency movements

### Formulating a Currency Mgt. Program

The strategic currency positioning of the portfolio should be biased toward a more-fully hedged currency management program the more:

- Short term the investment objectives of the portfolio
- Risk averse
- Immediate the income and/or liquidity needs of the portfolio
- Fixed-income assets are held in a foreign-currency portfolio
- Cheaply a hedging program can be implemented
- Volatile (risky) financial markets are

## Active (Tactical) Currency Management

Tactical decisions involve active currency management based on

- Economic fundamentals
- Technical analysis
- Carry trade
- Volatility trading

### Economic fundamentals

- The base currency's real exchange rate should appreciate (depreciation) if there is an upward (downward) movement in:
  - its long-run equilibrium real exchange rate
  - either its real or nominal interest rates, which should attract foreign capital
  - expected foreign inflation, which should cause the foreign currency to depreciate
  - the foreign risk premium, which should make foreign assets less attractive compared with the base currency nation's domestic assets

### Carry Trade

- The carry trade is a trading strategy of borrowing in low-yield currencies and investing in high-yield currencies
- When the base currency has a lower interest rate than the price currency, the base currency will trade at a forward premium
  - F~0~>S~0~
- Being a high-yield currency means trading at a forward discount
  - F~0~< S~0~
- Uncovered interest rate parity: $ \% \Delta S_{H/L} \approx i_H - i_L $
- **If uncovered interest rate parity holds,**
  - **The yield spread advantage for the high-yielding currency (the right side of the equation) will, on average, be matched by the depreciation of the high-yield currency** (the left side of the equation; the low-yield currency is the base currency and hence a positive value for % SH/L means a depreciation of the high-yield currency)
- uncovered interest rate parity asserts that, on a longer-term average, the return on an unhedged foreign-currency asset investment will be the same as a domestic-currency investment.
- But **in reality**, the historical data show that there are **persistent deviations from uncovered interest rate parity** in FX markets, at least in the short to medium term
- Long periods of market stability can make these extra returns enticing to many investors, and the longer the yield differential persists between high-yield and low-yield currencies, the more carry trade positions will have a tendency to build up
- Any time global financial markets are under stress there is a flight to safety that causes rapid movements in exchange rates, and usually a panicked unwinding of carry trades. As a result, traders running carry trades often get caught in losing positions, with the leverage involved magnifying their losses
- One guide to the riskiness of the carry trade is the volatility of spot rate movements for the currency pair; all else equal, **lower volatility is better for a carry trade position**
- This persistent violation of uncovered interest rate parity described by the carry trade is often referred to as the **forward rate bias**
  - Trading the forward rate bias involves buying currencies selling at a forward discount, and selling currencies trading at a forward premium
- The difference between carry trade and forward rate bias
  - Carry Trade: borrowing in low-yield currencies, investing in high yield currencies
  - Forward rate bias: Being low-yield currency and trading at a forward premium. Being high-yield currency means trading at a forward discount
- Summary

|                               |        Buy/invest         |       Sell/borrow        |
| :---------------------------: | :-----------------------: | :----------------------: |
| Implementing the carry trade  |    High-yield currency    |    Low-yield currency    |
| Trading the forward rate bias | Forward discount currency | Forward premium currency |

### Volatility Trading

- Delta Hedging
  - hedge away the option position's exposure to delta, the price risk of the underlying (the FX spot rate), which leads to a delta-neutral position
  - Delta shows the sensitivity of the option price to changes in the spot exchange rate
  - Typically implementing this delta hedge is done using either forward contracts or a spot transaction
  - Straddle
  - Strangle
    - a long position is buying out-of-the-money (OTM) puts and calls with the same expiry date and the same degree of being out of the money
    - cheaper
    - but require higher vol. to be profitable

## Tools of Currency Management

### Forward contract

- institutional investors prefer to use forward contracts for the following reasons
  - can be customized in
    - settlement dates
    - contract size
    - currency pair
  - no initial margin required
  - forward contracts are more liquid than futures
- Static hedge: unchanging hedge
- Dynamic hedge:rebalancing the portfolio periodically
- The **roll yield**, also called the **roll return**, on a hedge results from the fact that forward contracts are priced at the spot rate adjusted for the number of forward points at that maturity
$$ roll\;yield = \left | \frac{F_{P/B}-S_{P/B}}{S_{P/B}} \right | $$
- A positive roll yield results from buying the base currency at a forward discount or selling it at a forward premium

### Strategies to Reduce Hedging Costs & Modify Risk

- Over-/Under-Hedging using forward contracts
- Protective put using OTM options
- Risk reversal or collar
- Put spread
- Seagull spread
  - combine the original put spread position with a covered call position
  - be long a protective put and then write both a call and a deep-OTM put
- Exotic options

### Hedging Multiple Foreign Currencies

- Must consider the correlation between the various foreign-currency risk exposures
- **cross hedge**, also referred to a proxy hedge, occurs when a position in one asset (or a derivative based on the asset) is used to hedge the risk exposures of a different asset (or a derivative based on it).
- **Macro hedges** is more focused on the entire portfolio, particularly when individual asset price movements are highly correlated, rather than on individual assets or currency pairs

- Basis risk
  - any time a direct currency hedge (i.e., a spot rate hedged against its own forward contract) is replaced with an indirect hedge (cross hedge, macro hedge), basis risk is brought into the portfolio. 
  - Basis risk reflects the fact that
    - The price movements in the exposure being hedged and the price movements in the cross hedge instrument are **not perfectly correlated**
    - The **correlation will change with time**

## Currency Management of Emerging Markets

- Higher trading costs under "normal" market conditions
- The increased likelihood of extreme market events and severe illiquidity under stressed market conditions

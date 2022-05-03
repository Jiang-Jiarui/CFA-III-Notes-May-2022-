# Capital Market Expectation

[TOC]

## Part 1: Framework and Macro Considerations

### Challenges when formulating CME

#### What is CME?

- Capital market expectations are risk and return expectations regarding  classes of assets
- Cross-sectional consistency
- Inter-temporal consistency

#### Challenges in Forecasting

1. Limitations to using economic data
   - **Time Lag** of the data
   - Data might be **revised** in the future (including methodology)
   - Data index are often **rebased** overtime
2. Data measurement errors and biases
   - Transcription errors
   - Survivorship bias
   - Appraisal data: underestimate the Vol
3. Limitations of historical estimates
    - regime changes -> nonstationary data
    - Non-stationarity: statistical property change over time
    - long time period is preferable for several reasons:
       - statistically required
       - smaller variance to the estimates
       - asynchronous data: can cause distorted correlation
4. Ex Post risk as a biased risk measure of Ex Ante risk
    - Using ex post data (after the fact) to determine ex ante (before the fact) risk and return can be problematic
      - underestimate the risks
      - overestimate their potential returns
    - data series includes even one observation of a rare event, we may substantially overstate the likelihood of such events happening in the future
5. Analyst Methods Bias: non-robust pattern
    - Data-mining
    - Time-period bias
6. Failure to account for conditioning information
7. Misinterpretation of Correlations
8. Psychological biases
9. Model uncertainty
    - **Model uncertainty**: refers to selecting the correct model
    - **Parameter uncertainty**: refers to estimation errors in model parameters
    - **Input uncertainty**: refers to knowing the correct input values for the model

### The trend rate of growth

#### Exogenous Shocks to Growth

- Exogenous shocks:unanticipated events that occur outside the normal course of an economy
  - likely produce statistical regime changes

#### Decomposition of GDP Growth

- The trend growth in GDP is the sum of the following
  - Growth from labor inputs
    - growth in potential labor force size
    - growth in actual labor force participation
  - Growth from labor productivity
    - growth from capital inputs
    - total factor productivity (TFP) growth

#### Anchoring Asset Returns to Trend Growth

- The trend growth rate also provides an anchor for long-run equity appreciation
  - We can express the aggregate market value of equity, V~e~, as the product of three factors: the level of nominal GDP, the share of profits in the economy, S~k~ (earnings/GDP), and the P/E ratio (PE)
  - $V_e = GDP *S_k*PE$
  - The growth rate of the total value of equity in an economy is linked to the growth rate of GDP

### Approaches to economic forecasting

- econometric modeling
- economic indicators
- checklist approach

### The business cycle

#### Business Cycle Analysis

The business cycle can be subdivided into five phases：

- Initial recovery
  - Falling inflation
  - Low or falling short-term interest rates
- Early expansion
- Late expansion
- Slowdown
- Contraction

#### Inflation Implications

- Inflation: generally rising prices
- Disinflation: deceleration in the rate of inflation
- Deflation: generally falling prices

| Business Cycle   | Inflation                                              | Economic Policy           | Markets                                                      |
| ---------------- | ------------------------------------------------------ | ------------------------- | ------------------------------------------------------------ |
| **Initial recovery** | Initially declining inflation                          | Stimulative               | - Short-term rates low or declining <br/>Long-term rates bottoming and bond prices peaking<br/>- Stock prices increasing |
| **Early expansion**  | Low inflation and good economic growth                 | Becoming less stimulative | - Short-term rates increasing<br/>- Long-term rates bottoming or increasing with bond prices beginning to decline<br/>- Stock prices increasing |
| **Late expansion**   | Inflation rate increasing                              | Becoming restrictive      | - Short-term and long-term rates increasing with bond prices declining<br/>- Stock prices peaking and volatile |
| **Slowdown**         | Inflation continues to accelerate                      | Becoming less restrictive | - Short-term and long-term rates peaking and then declining with bond prices starting to increase<br/>- Stock prices declining |
| **Contraction**      | Real economic activity declining and inflation peaking | Easing                    | - Short-term and long-term rates declining with bond prices increasing<br/>- Stock prices begin to increase later in the recession |

</br>

|                                            | Cash  Equivalents                                            | Bonds                                                        | Equity                                                       | Real Estate                                                  |
| ------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Inflation  within expectations**         | Earn  the real rate of interest                              | Shorter-term  yields more volatile than longer-term yields   | No  impact given predictable economic growth                 | Neutral  impact with typical rates of return                 |
| **Inflation  above or below expectations** | Positive  (negative) impact with increasing (decreasing) yields | Longer-term  yields more volatile than shorter-term yields   | Negative  impact given the potential for central bank action or falling asset prices,  though some companies may be able to pass rising costs on to customers | Positive  impact as real asset values increase with     inflation |
| **Deflation**                              | Positive  impact if nominal interest rates are bound by 0%   | Positive  impact as fixed future cash flows have greater purchasing power (assuming no  default on the bonds) | Negative  impact as economic activity and business declines  | Negative  impact as property values generally decline        |

### Monetary policy and fiscal policy

- Most central banks strive to balance price stability against economic growth. The ultimate goal is to keep growth near its **long-run sustainable rate**, because growth faster than the long-run rate usually results in increased inflation
- The equilibrium interest rate in a country (the rate at which a balance between growth and inflation is achieved) is referred to as the **neutral rate**
  - It is generally thought that the **neutral rate** is composed of an **inflation component** and a **real growth component**
- **Taylor rule**：determines the target interest rate using the neutral rate, expected GDP relative to its long-term trend, and expected inflation relative to its targeted amount
  - $$
   i^* - \pi_e= r_{neutral} +  0.5*(\hat{Y}_e-\hat{Y}_{trend})+0.5*(\pi_e-\pi_{target})
   $$
  - i^*^ is the target nominal policy rate
- Negative interest rate
- Fiscal Policy
  - it is not the level of the budget deficit that matters - it is the **change in the deficit**
  - changes in the deficit that occur naturally over the course of the business cycle **are not stimulative or restrictive**
- The Yield Curve
  - The yield curve demonstrates the relationship between interest rates and the maturity of debt securities
  - The curve is **sensitive to government actions as well as current and expected economic conditions**

### International Considerations

- **Macroeconomic links** can produce convergence in business cycles among economies
  - International trade
  - International capital flows
  - Interest rates
  - currency exchange rates

</br>

## Part 2: Forecasting Asset Class Returns

### Forecasting Fixed Income return

#### DCF model

- useful when there are **known future cash flows**, or when cash flows can be **estimated accurately**
- The DCF analysis supports the use of yield to maturity (YTM) as an estimate of expected return
- YTM is the discount rate that makes the present value of future cash flows equal to the bond's price. It will be the realized return earned if:
  - cash flows are **reinvested at the YTM** and
  - the bond is **held to maturity**
- Reasons why the bond's realized return may deviate from the initial YTM
  - sell the bond prior to maturity, generating a capital gain or loss
  - rising or falling interest rates may result in not only changing bond prices, but **changing reinvestment returns**
    - falling (rising) interest rates will decrease (increase) reinvestment returns. The overall gain or loss to the investor will depend on the **investment horizon.**
    - **For an investment horizon longer than the Macaulay duration, the reinvestment risk dominates, meaning that falling (rising) interest rates will result in a lower (higher) realized return.**

#### Risk Premium Approach

- Risk premium approcach starts with a **risk-free rat**e and then **adds compensation for additional risks**
- one-period default-free rate
  - The short-term default-free rate matches the forecast horizon and is calculated from the most liquid instrument
  - it is closest to the **government zero-coupon yield** and is closely tied to the central bank policy rate
  - **Futures contract rates** provide useful proxies for this expected path of short-term interest rates
- term premium
  - can be observed from spot yield curve
  - four main drivers of the term premium
    - inflation uncertainty
    - recession hedge
    - supply and demand
    - business cycles
- credit premium
  - The credit premium compensates for the **expected level of losses** and for the **risk of default losses**, both of are parts of the **credit spread**
- liquidity premium
  - Securities with the highest liquidity are the newest sovereign bond issues, current coupon mortgage-backed securities, and some high quality corporate bonds.
  - Liquidity is higher for bonds that are (1) issued at close to par or market rates, (2) new, (3) large in size, (4) issued by a frequent and well-known issuer, (5) simple in structure, and (6) of high credit quality

### Forecasting Equity return

#### Grinold-Kroner model

- $$E(R_e)= (D/P-\%\Delta S) + \%\Delta E +\%\Delta P/E$$
- $\%\Delta S$ is the expected percent change in shares outstanding
- The **expected cash flow return (income return)**:$(D/P-\%\Delta S)$
- The **expected nominal earnings growth** is the real growth in earnings plus expected inflation: $\%\Delta E$
- The **expected repricing return** is captured by the expected change in the P/E ratio:$\%\Delta P/E$

#### Singer-Terhaar model

- The Singer-Terhaar model is based on two versions of the international Capital Asset Pricing Model (CAPM): one in which global asset markets are **fully integrated**, and another in which markets are **fully segmented**
- First Component: **Fully Integrated CAPM**:$$ RP_i^G=\beta_{i,GM}*RP_{GM}=\beta_{i,GM}*\sigma_i(\frac{RP_{GM}}{\sigma_{GM}})$$
- Second Component: **Fully Segmented CAPM** :$$RP_i^G = 1*\sigma_i(\frac{RP_i^s}{\sigma_i})$$
- The combination: **Weighted CAPM depending on the level of integration $\varphi$**: $$RP_i=\varphi RP_i^G+(1-\varphi)RP_i^S$$

### Forecasting Real Estate return

- Each property is part of a **heterogeneous** group with its unique characteristics
- Calculating returns is often done through **appraisals**, which are subject to time lags and data smoothing
- Capitalization rate (cap rate), is a commercial property's earning yield
  - $ cap ~ rate = \frac{current ~NOI}{property~value}$
  - $ cap~rate = E(R_{re})-NOI~growth~rate$
  - $ E(R_{re})=cap~rate +NOI~growth~rate$
- If an investor has a finite time period:
  - $ E(R_{re})=cap~rate +NOI~growth~rate - \%\Delta cap~rate$
- the cap rate is used as a **long-term discount rate** for real estate property valuations
- Cap rates are **positively related** to changes in interest rates and vacancy rates.
- They are **inversely related** to the availability of credit and the availability of debt financing
- Risk Premiums related to real estate
  - Term premium
  - Credit premium
  - Equity risk premium
- Adjustments required
  - Impact of smoothing must be removed
  - Illiquidity of real estate must be adjusted
- REITS
  - generally strongly correlated with equities in the short term
  - Over long time horizons, REITs have a relatively high correlation with direct real estate
  - Given that REITs use significant leverage, their returns and risks must be first unlevered
- Residential real estate: outperform equities on an inflation-adjusted basis with lower volatility

### Forecasting Exchange rate

- Trade in goods and services affects exchange rates through:
  - trade flows
  - PPP: prices of goods and services should reflect changes in exchange rates. As a result, the exchange rate movement should follow the expected inflation rate differentials
  - comptetiveness and sustainability of the current account
- Capital mobility
  - The expected percentage change in the exchange rate can be computed as the difference between nominal short-term interest rates and the risk premiums of the domestic portfolio over the foreign portfolio
  - $$ E(\%\Delta S_{d/f})=(r_d-r_f)+(Term_d-Term_f)+(Credit_d-Credit_f)+(Equity_d-Equity_f)+(Liquid_d-Liquid_f) $$
- **Uncovered interest rate parity (UIP)**:UIP states that exchange rate changes should equal differences in nominal interest rates. Carry trades are considered to be successful because they include a risk premium, confirming the validity of the risk premiums in the equation

### Forecasting Volatility

- Variance-covariance(VCV) matrix
- Factor-based VCV matrices
  - significantly reduces the number of required observations
- ARCH model
  - $$\sigma ^2_t = \gamma+\alpha\sigma ^2_{t-1}+\beta\eta ^2_t
  $$

# CH3 Asset Allocation and Related Decisions in Portfolio Management

[toc]

## Overview of Asset Allocation

### The portfolio management Process

#### Initial Flow

- Identify and articulate the asset owner's objectives
- Document **objective and constraints** in the investment policy statement (**IPS**)
- Develop capital market expectations for the **planning horizon**
- Structure Portfolio
- Evaluate progress toward achieving objectives and compliance with IPS

#### Feedback Flows

- Identify changes the asset owner's economic balance sheet, objectives, or constraints
- Monitor prices and markets

### Investment governance

- **Investment governance** represents the organization of decision-making responsibilities and oversight activities
- Important aspects of an effective investment governance model
  - **Articulating Investment Objectives**
    - long- and short-term objectives
    - Unique return requirements and risk sensitivities
  - **Allocation of Rights and Responsibilities**
    - Governing investment committee
    - Investment staff
    - Third-Party staff
  - Investment Policy Statement
  - Asset Allocation and Rebalancing Policy
  - Reporting Framework
  - Governance Audit

### Economic balance sheet

- Other than items shown in conventional B/S sheet, Economic B/S sheet also includes Additional/Extended asset and liability items, ie. **PV of expected future income/liabilities**
- Additional/Extended asset and liability are relevant in making Asset Allocation process, but not appear on conventional balance sheets

![Economic Balance Sheet](./Asset/Economic%20Balance%20Sheet.png)

- Extended portfolio assets
  - For individual investor
    - Human capital (The PV of future earnings)
    - The PV of pension income
    - The PV of expected inheritances
  - For institutional investor
    - Underground mineral resources
    - The PV of future intellectual property royalties
- Extended portfolio liabilities
  - For individual investor
    - The PV of future consumption
  - For institutional investors
    - The PV of prospective payouts for foundations

### Asset allocation approaches

- **Asset-only**: Mean variance optimization (MVO)
- **Liability-relative**: Funding liabilities
- **Goals-based**: Achieving the goals

#### Objectives:

| Asset Allocation Approach | Typical Objectives                                     |
| :-----------------------: | :----------------------------------------------------: |
| **Asset-Only**                | Maximize **Sharp Ratio** for acceptable level of vol.       |
| **Liability-relative**        | Fund liabilities and invest excess assets for growth    |
| **Goal Based**                | Achieve goals with specified required prob. of success |
  
#### Risk Concepts

| Asset Allocation Approach | Risk Measures                                                |
| :-----------------------: | ----------------------------------------------------------- |
| **Asset-Only**               | - **Vol (std.)**<br />- Tracking Error<br />- Downside risk incl: semi-var, maixmum drawdown, VaR |
| **Liability-relative**        | - Shortfall risk<br />- Vol. of contributions needed to fund liabilities<br />- std. of the surplus |
| **Goal Based**                | Maximum accepatable probabilitu of not achieving a goal     |

#### Asset Class

- Three "Super Class" of assets
  - Capital Assets (提供收入)
    - Provide an ongoing source of value
    - can be valued by NPV
  - Consumable/transformable assets (生产性资料)
    - such as commodities
  - Store of value (保值)
    - Currencies and art
- Criteria for specifying asset classes
  - Assets within an asset class should be relatively homogeneous;
  - Asset classes should be mutually exclusive;
  - Asset classes should be diversifying;
  - The asset classes as a group should make up a preponderance of world investable wealth;
  - Asset classes selected for investment should have the capacity to absorb a meaningful proportion of an investor's portfolio

#### Risk Factor

- Asset-based asset allocation
  - Modeling using asset classes as the unit of analysis tends to obscure the portfolio's sensitivity to overlapping risk factors
- Factor-based asset allocation
  - Process of factor-based asset allocation
    - Specify risk factors and the desired exposure to each factor
    - Describe asset classes with respect to their sensitivities to each of the factors
    - Construct factor portfolios that isolate exposure to the risk factor
    - Map back a choice of risk exposures in factor space to asset class space for implementation
- How risk factor exposures can be achieved by long and short positions or use existing instrument
  - **Inflation**
    - Going long nominal Treasuries and short inflation-linked bonds isolates the inflation component
  - **Real interest rates**
    - Inflation-linked bonds provide a proxy for real interest rates
  - **US volatility**
    - VIX
  - **Credit spread**
    - Going long high-spread credit bond and short Treasuries/government bonds isolates credit exposure
  - **Duration**
    - Going long 10+ year Treasuries and short 1 3 year Treasuries isolates the duration exposure being targeted.

#### Global Market Portfolio

- Global market portfolio sums all investable assets (global stocks, bonds, real estate, and so forth) held by investors, and reflects the balancing of supply and demand across world markets
- Global market-value weighted portfolio should be considered as a baseline asset allocation in an asset-only approach.

### Strategic Asset Allocation

- SAA: An asset allocation that arises in long-term investment planning
- Utility function
  - Mean-Variance utility: $U = E(r_p)-\frac{1}{2}\lambda\sigma^2_p$
- The simplest asset allocation decision problem involves <u>one risky asset and one risk-free asset</u>. Let λ, μ, r~f~, and σ^2^ represent, respectively, the investor’s degree of risk aversion, the risk asset’s expected return, the risk-free interest rate, and the variance of return. With mean–variance utility, **the optimal allocation to the risky asset, $w^*$, can be shown to equal**
$$ w^*= \frac{1}{\lambda}(\frac{\mu-r_f}{\sigma^2})
$$
- Process of selecting strategic asset allocation
  - Determine and quantify the investor’s objectives
  - Determine the investor’s risk tolerance and how risk should be expressed and measured
  - Determine the investment horizon(s)
  - Determine other constraints and the requirements they impose on asset allocation choices
  - Determine the approach to asset allocation that is most suitable for the investor
  - Specify asset classes, and develop a set of capital market expectations for the specified asset classes
  - Develop a range of potential asset allocation choices for consideration
  - Test the robustness of the potential choices

### Strategic implementation choices

- Tactical asset allocation (TAA): involves deliberate short-term deviations from the strategic asset allocation
- Two dimensions of passive/active choices
  - Passive/active management of the strategic asset class weights;(whether to deviate from the SAA tactically or not)
  - Passive and active management of allocations to asset classes
- Passive/Active Management of Asset Class Weights
  - Tactical asset allocation TAA
    - involves deliberate short-term deviations from the strategic asset allocation
      - Deviation restricted by risk budgets or rebalance range
        - Risk budget: address which risk to take and how much of each to take
      - Responsive to price momentum, business cycle , asset class valuation, etc
      - Tradeoff between potential outperformance and tracking error
      - Key limitation: additional trading, monitor cost and CG tax
  - Dynamic asset allocation DAA?
- Factors influencing where to invest on the passive/active spectrum
  - Available investments
  - Scalability of active strategies being considered
  - The feasibility of investing passively while incorporating client-specific constraints
  - Beliefs concerning market informational efficiency
  - The trade-off of expected incremental benefits relative to incremental costs and risks of active choices
  - Tax status

### Strategic considerations in rebalancing

- **Rebalancing:** adjust portfolio weights to more closely align with the strategic asset allocation
- **Approaches to rebalancing**
  - Calendar rebalancing: on a periodic basis
  - Percent-range rebalancing (range-based rebalance)
    - Trigger points or Rebalance range (or corridor)
- **Frequency of the portfolio valued**
  - The narrower corridor, the more frequent rebalance
  - The more frequent the monitoring, the greater the precision in implementation
  - **Fully or partially correcting**
    - Rebalance back to target weights
    - Rebalance to range edge
    - Rebalance halfway between the range-edge trigger point and the target weight
  - **Factors affecting the optimal corridor width of an asset class**
    - Transaction cost
    - Risk tolerance
    - Correlation
    - Volatility
    - Liquidity
    - Taxes
  - Disciplined rebalancing has tended to reduce risk while incrementally adding to returns
  - Rebalancing earns a return from being short volatility

## Principles of Asset Allocation

### Developing asset-only asset allocations

#### MVO

- ![MVO](Asset\MVO.png)
- MVO requires three sets of inputs: **returns**, **risks (standard deviations)**, and **pair-wise correlations** for the assets in the opportunity set, and the objective function expressed as follows
$$U_m = E(R_m)-0.5\lambda\sigma^2_m
$$
- Some issues to consider regarding MVO
  - Common constraints
    - The simplest optimization places no constraints on asset class weights except the budget constraint that weights sum to 1.
    - The non-negativity constraint leads to corner-portfolio EF
- Strengths
  - Most common and widely used
  - Basis for more sophisticated approaches
- Weaknesses
  - The asset allocations tend to be highly concentrated in a subset of the available asset classes; (add constraints)
  - The outputs (asset allocations) are highly sensitive to small changes in the inputs; (Resampled MVO, Reversed MVO and Black-Litterman Model)
  - Investors are often concerned with characteristics of asset class returns such as skewness and kurtosis that are not accounted for in MVO; (Non-normal optimization approaches)
  - The MVO may ignore the effect of illiquidity (Three additional methods)
  - While the asset allocations may appear diversified across assets, the sources of risk may not be diversified; (Risk budgeting and Factor-based model)
  - MVO is a single-period framework that does not take account of trading/ rebalancing costs and taxes;(MCS method)
  - MVO allocations may have no direct connection to the factors affecting any liability or consumption streams;

#### Addressing the criticisms of MVO

##### Add constraints

- Typical constraints
  - Budget
  - non-negativity
- Additional constraints
  - Specify a set allocation to a specific asset
  - Specify an asset allocation range for an asset
  - Specify an upper limit, due to liquidity considerations
  - Specify the relative allocation of two or more assets

##### Resampled MVO, Reverse optimization, Black-Litterman Model

###### Resampled MVO

- Resampled MVO: combine traditional MVO with MCS
- leads to more diversified asset allocation
- less sensitive to changes in input variables
  - criticism
    - Some frontier have concave "bumps"
    - the riskier asset allocations are over-diversified
    - the asset allocations inherit the estimation errors in the original inputs

###### Reverse optimization

- Inputs
  - global market portfolio that are assumed to be optimal
  - covariance
  - risk aversion coefficient
- Output
  - Expected returns (implied return)
  - process:
![Reverse optimization](Asset/Reversed%20optimization.png)

###### Black-Litterman model

- Process
  - Starts with excess returns (in excess of the risk-free rate) produced from reverse optimization
  - And then provides a technique for altering reverse-optimized expected returns in such a way that they views.
  - A new MVO is run
- Strength
  - Enable investor to combine their unique forecasts
  - Asset allocation grounded in market capitalization, reflect market expectation (highly diversified portfolio, avoid concentration)
![BL model](Asset/Black-Litterman%20Model.png)

##### Non-normal optimization

consider the non-normal return distribution characteristics and use a more sophisticated definition of risk, such as:

- Mean semivariance optimization
- Mean conditional value-at-risk optimization
- Mean variance-skewness optimization
- Mean variance-skewness-kurtosis optimization

##### Liquidity consideration

In addressing asset allocation involving less liquid asset classes, practical options include the following

- (1) Exclude less liquid asset classes from the asset allocation decision and then consider real estate funds, infrastructure funds, and private equity funds as potential implementation vehicles when fulfilling the target strategic asset allocation
- Include less liquid asset classes in the asset allocation decision and attempt to model the inputs to represent the specific risk characteristics associated with the likely implementation vehicles

##### Factor-Based Asset Allocation

Factor-based asset allocation also requires three sets of inputs: returns, risks (standard deviations), and pair-wise correlations for these factors in the opportunity set, in order to get an optimized solution.

##### MCS

- Monte Carlo simulation complements MVO by addressing the limitations of MVO as a single-period framework

### Developing liability-relative asset allocation

#### Surplus Optimization

- adapting asset-only mean variance optimization to an efficient frontier based on the volatility of surplus by substituting surplus return for asset return over any given time horizon, all else equal

#### Hedging/Return-seeking portfolio

- In this approach, the liability-relative asset allocation task is divided into two parts, thus this approach is also called two-portfolio approach
- The hedging portfolio must include assets whose return are driven by the same factors that drive the returns of the liabilities

#### Integrated Asset-Liability Approach

- The approach, integrating the liability portfolio with the asset portfolio, requires a formal method for selecting liabilities and for linking the asset performance with changes in the liability values

![comparing](Asset/Comparing%20LD%20AA.png)

### Developing goals-based asset allocations

- Disaggregates the investor s portfolio into a number of sub-portfolios, each of which is designed to fund an individual goal (or mental account with its own time horizon and required probability of success.
- Goals-based asset allocation applies best to individuals who have multiple goals, time horizons, and urgency levels.
- Constructing sub-portfolio
  - determine discount rate
    - time horizon
    - required probability of success
  - allocate capital to sub-portfolios
    - ==According to each client goal, pick the highest probability- and horizon adjusted discount rates to discount the expected cash flows, and then obtain the lowest initially required capital for each goal==
  - excess capital

### Heuristics and other approaches

- "120 minus your age" rule
- 60/40 stock/bond heuristic
- Endowment model (Yale model)
- 1/N rule

### Risk budgeting and Risk Parity

- A **risk budget** is simply a particular allocation of portfolio risk which distributes risk across assets in the portfolio
- The **goal of risk budgeting** is to maximize return per unit of risk whether overall market risk or active risk
- The risk **budgeting process** is the process of identifying the **total amount of risk** and **find an optimal risk budget**
- **Marginal Contribution to Total Risk (MCTR):** identifies the rate at which risk would change with a small (or marginal) change in the current weights of an asset class
  - MCTR = Asset beta relative to portfolio $\times$ Portfolio standard deviation
$$ MCTR=\beta_i\times\sigma_p
$$
- **Absolute Contribution to Total Risk (ACTR):** measures how much an asset class contributes to portfolio return volatility
$$ ACTR=w_i\times MCTR=w_i \times \beta_i \times \sigma_p
$$
- **An asset allocation is optimal** when the MCTR is the same for all assets in the portfolio
- **Risk Parity**
  - A risk parity asset allocation is based on the notion that each asset (asset class or risk factor) should contribute equally to the total risk of the portfolio for a portfolio to be well diversified.
$$ACTR = w_i\beta_i\sigma_i=\frac{1}n{\sigma_p}
$$
  - Advantage
    - The sources of risk are diversified (asset classes)
    - Back tests of levered risk parity portfolios have produced promising results
  - Disadvantage
    - ignores expected returns
    - The contribution to risk is highly dependent on the formation of the opportunity set
    - Back tests argue that they suffer from look-back bias
    - Dependent on the ability to use extremely large amounts of leverage at low borrow rates

## Asset Allocation with Real-World Constraints

### Constraints on asset allocation

![constraints](Asset/Constraints%20in%20Asset%20Allocation.png)

### Tax considerations in asset allocation

#### After-tax portfolio optimization

$$r_{at}=p_dr_{pt}(1-t_d)+p_dr_{pt}(1-t_{cg})
$$

$$\sigma_{at}=\sigma_{pt}(1-t)
$$

$$R_{at} =R_{pt}/(1-t),R\;is\;rebalancing\;range
$$

- Strategies to Reduce Tax Impact
  - Tax loss harvesting refers to sell securities in loss statue along with the selling of profitable securities when realize profit
  - Place less tax-efficient assets in accounts with more favorable tax treatment
    - general rule: place bonds in tax deferred account, and put stocks in taxable account

### Revisions to asset allocation

All asset owners should affirm annually that the asset allocation remains appropriate given their needs and circumstances
- A change in goals
- A change in constraints
- A change in beliefs

### Short-term shifts in asset allocation

- Tactical asset allocation (TAA) allows short-term deviations from SAA targets
- Most common ways to evaluate TAA decisions are:
  - A comparison of the Sharpe ratio realized under the TAA relative to the Sharpe ratio that would have been realized under the SAA
  - Evaluating the information ratio
  - The t-statistic of the average excess return of the TAA portfolio relative to the SAA portfolio
  - Plotting the realized return and risk of the TAA portfolio versus the realized return and risk of portfolios along the SAA's efficient frontier
- Two major approaches to TAA

| Discretionary TAA                                            | Systematic TAA                                               |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| Discretionary TAA is predicated on the existence of manager skill in predicting and timing short-term market moves away from the expected outcome for each asset class that is embedded in the SAA policy portfolio | Using signals, systematic TAA attempts to capture asset class level return anomalies that have been shown to have some predictability and persistence. |  


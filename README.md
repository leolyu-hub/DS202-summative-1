[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/-Ovub_m9)
# 📝 DS202W W08 Summative

**author: Dr. [Ghita Berrada](https://www.lse.ac.uk/DSI/People/Ghita-Berrada)**


⏲️ **Due Date**:

- 11 March 2026 at 5pm (London time)

If you update your files on GitHub after this date without an authorised extension, you will receive a [late submission penalty](https://info.lse.ac.uk/current-students/services/assessment-and-results/exams/exam-discipline-and-academic-misconduct).

Did you have an extenuating circumstance and need an extension? Send an e-mail to 📧 [Kevin](mailto:DSI.ug@lse.ac.uk?subject=DS202W%20-%20W07%20Summative%20Extension)

🎯 **Main Objectives:**

- Demonstrate your ability to write a report in Quarto Markdown
- Demonstrate your ability to fit a linear/logistic regression model
- Demonstrate your ability to interpret and evaluate the performance of a linear/logistic regression model
- Demonstrate your understanding of supervised learning techniques
- Demonstrate your ability to defend your model choices

⚖️ **Assignment Weight**:

This assignment is worth 30% of your final grade in this course.

<img src="https://img.shields.io/badge/30%25-c63c4a?style=for-the-badge&logoColor=white" alt="30%">

>[!IMPORTANT]
>## Do you know your CANDIDATE NUMBER? You will need it.
>
> _"Your candidate number is a unique five digit number that ensures that your work is marked anonymously. It is different to your student number and will change every year. **Candidate numbers can be accessed using LSE for You.**"_ 
>
> Source: [LSE](https://www.lse.ac.uk/accounting/study/New-Arrival/Exams-and-Assessments)

# 📝 Instructions

1. Go to our Slack workspace's `#ds202w-central` channel to find a GitHub Classroom link. Do not share this link with anyone outside this course!

2. Click on the link, sign in to GitHub and then click on the green button `Accept this assignment`.

3. You will be redirected to a new private repository created just for you. The repository will be named `ds202w-2025-2026-w08-summative--yourusername`, where `yourusername` is your GitHub username. The repository will be private and will contain a `README.md` file with a copy of these instructions.

4. Recall what is your LSE CANDIDATE NUMBER. You will need it in the next step. 

5. Create your own `<CANDIDATE_NUMBER>.qmd` file with your answers, replacing the text `<CANDIDATE_NUMBER>` with your actual LSE number. 

You can create a `.qmd` file from a Jupyter notebook (i.e `.ipynb`) by going on the VSCode Terminal, making sure you are in the same directory as your Jupyter notebook (use the `pwd` to check which directory you're in and `cd` command to change directory if needed) and then typing the following command:

```zsh
quarto convert <CANDIDATE_NUMBER>.ipynb
```

where `<CANDIDATE_NUMBER>.ipynb` is the name of the Jupyter notebook you want to convert into `.qmd`

Also check out the [Quarto documentation](https://quarto.org/docs/tools/vscode-notebook.html) to better understand the conversion from `ipynb` to `qmd`.

And check out [this tutorial](https://education.launchcode.org/intro-to-professional-web-dev/appendices/terminal-commands/terminal-commands-tutorial.html) if you want to better understand the commands you can run on your VSCode terminal (e.g to change current directory).

You can also use the `.qmd` file you used in the W01 lab as a template. Just remove anything that is not relevant to this assignment. 

6. Then, replace whatever is between the `---` lines at the top of your newly created `.qmd` file with the following:

    ```yaml
    ---
    title: "DS202W - W08 Summative"
    author: <CANDIDATE_NUMBER>
    output: html
    self-contained: true
    jupyter: python3
    engine: jupyter
    editor:
      render-on-save: true
       preview: true
    ---
    ```

    Once again, replace the text `<CANDIDATE_NUMBER>` with your actual LSE CANDIDATE NUMBER. For example, if your candidate number is `12345`, then your `.qmd` file should start with:

    ```yaml
    ---
    title: "DS202W - W08 Summative"
    author: 12345
    output: html
    self-contained: true
    jupyter: python3
    engine: jupyter
    editor:
      render-on-save: true
      preview: true
    ---
    ```

8. Fill out the `.qmd` file with your answers. Use headers and code chunks to keep your work organised. This will make it easier for us to grade your work. Learn more about the basics of **markdown formatting** [here](https://quarto.org/docs/authoring/markdown-basics.html).

7. Use the `#help` channel on Slack liberally if you get stuck.  

9. Once you are done, click on the `Render` button at the top of the `.qmd` file. This will create an `.html` file with the same name as your `.qmd` file. For example, if your `.qmd` file is named `12345.qmd`, then the `.html` file will be named `12345.html`. 

    Ensure that your `.qmd` code is reproducible, that is, if we were to restart VSCode and run your notebook from scratch, from top to the bottom, we would get the same results as you did.

10. Push both files to your GitHub repository. You can push your changes as many times as you want before the deadline. We will only grade the last version of your assignment. Not sure how to use Git on your computer? You can always add the files via the GitHub web interface.

11. Read the section **How to get help and how to collaborate with others** at the end of this document.

## "What do I submit?"

You will submit two files:

- A Quarto markdown file with the following naming convention: `<CANDIDATE_NUMBER>.qmd`, where `<CANDIDATE_NUMBER>` is your candidate number. For example, if your candidate number is `12345`, then your file should be named `12345.qmd`.

- An HTML file render of the Quarto markdown file. To generate a render, the easiest way is to include these lines
  
```yaml
editor:
  render-on-save: true
  preview: true
```

in your `.qmd` header so that an HTML file is generated each time you preview your document (make sure you also have the Quarto extension installed in VSCode so that you do the preview by clicking on a button at the top right corner of the VSCode menu bar without having to use the Terminal!). Also, don't forget to add the line ```self-contained: true``` to your `.qmd` header, otherwise none of your plots will show!

Your `.qmd` header should look something like this:

```yaml
---
title: "✏️ W08 Summative"
author: <CANDIDATE_NUMBER>
format: html
self-contained: true
jupyter: python3
engine: jupyter
editor:
  render-on-save: true
  preview: true
---

```

- An HTML file render of the Quarto markdown file. **Make sure your file is self-contained (i.e figures are embedded within it)**

You don't need to click to submit anything. Your assignment will be automatically submitted when you `commit` **AND** `push` your changes to GitHub. You can push your changes as many times as you want before the deadline. We will only grade the last version of your assignment. Not sure how to use Git on your computer? You can always add the files via the GitHub web interface.

>[!IMPORTANT]
>### Formatting expectations
>
>Your document should:
>
>- Be clearly structured using section headings.
>
>- Combine code, output, and written interpretation in a coherent way.
>
>- Contain clearly labelled figures and tables where appropriate.
>
>- Include sufficient explanation for a reader to understand:
>
>  - your data construction decisions,
>
>  - your modelling choices,
>
>  - your evaluation strategy,
>
>  - and your conclusions.
>
> Code should support your analysis — it should not replace explanation.

# 📋 Your tasks

**What do we actually want from you?**

>[!IMPORTANT]
> ## General guidelines
>1. **Model selection matters:** You should make **clear, justified choices** about which models to use. **Resist the temptation to try every model you know!** State your modelling hypotheses clearly, justify your choices, and select only a few models to explore (more models does not mean a better grade!).
>2. **Dimensionality reduction:** You may use PCA, UMAP, or similar techniques if you think it helps your modelling. You must justify their use. These are optional.
>3. **Justification is crucial:** Simply presenting code without explanation will not get you high marks. **In fact, simply lining up code with no or little explanation is a fail.** You must justify your modelling choices (e.g., why a model is suitable for the dataset and problem context, how parameters were set), and interpret results and metrics **in context**.
>4. **Evaluation:** For all models, evaluate performance and justify your choice of metrics or evaluation strategy. Do not assume a single metric suffices for all conclusions.


## Part 1: Predicting Next-Month Gold Returns (50 marks)

Gold is often described as a hedge against inflation and a “safe haven” during periods of financial stress. Because gold does not generate cash flows (unlike bonds or equities), its valuation is closely linked to real interest rates, inflation expectations, global uncertainty, currency movements, and financial conditions. That makes gold an interesting forecasting target: its dynamics may reflect macroeconomic conditions, risk sentiment, currency movements, and global real activity.

In this part, you will build models to **predict next-month gold returns** using macro-financial indicators.

### 1.1 Data

You are provided with two datasets:

#### 📥 Main monthly dataset

[![Download CSV](https://img.shields.io/badge/Download-monthly_indicators_dataset_(csv_file)-b284be?style=for-the-badge&logo=download)](gold_price_prediction_dataset.csv)

Contains monthly gold prices and a set of macro-financial predictors.

#### 📥 Weekly financial conditions dataset

[![Download CSV](https://img.shields.io/badge/Download-NFCI_data_(csv_file)-b284be?style=for-the-badge&logo=download)](nfci-data-series-csv.csv)

Contains the Chicago Fed National Financial Conditions Index (weekly frequency).

You must integrate both datasets into a single modelling dataset.


### 1.2 Indicators

The economic and financial indicators available are as follows:

<table style="border-collapse:collapse; width:100%; border:2px solid #999;" border="1">
  <thead style="background-color:#f2f2f2;">
    <tr>
      <th style="padding:10px; border:1px solid #999;"><strong>Indicator (dataset variable)</strong></th>
      <th style="padding:10px; border:1px solid #999;"><strong>Meaning</strong></th>
      <th style="padding:10px; border:1px solid #999;"><strong>Source</strong></th>
    </tr>
  </thead>
  <tbody>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>Gold price</strong> (<code>gold_price</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Monthly gold futures price (USD). This is used to construct the return series that you will predict.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://uk.investing.com/commodities/gold-historical-data">Investing.com – Gold Futures Historical Data</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>US 10-Year Treasury Yield</strong> (<code>us_10y_yield</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        The yield investors receive on 10-year US government bonds. Higher yields increase the opportunity cost of holding non-yielding assets like gold.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://fred.stlouisfed.org/series/GS10">FRED: GS10</a>
      </td>
    </tr>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>10-Year Breakeven Inflation</strong> (<code>us_10y_breakeven_inflation</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Market-implied inflation expectations derived from Treasury Inflation-Protected Securities (TIPS).
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://fred.stlouisfed.org/series/T10YIEM">FRED: T10YIEM</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>Trade-Weighted US Dollar Index</strong> (<code>usd_broad_index</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Broad index of US dollar strength against major trading partners. Since gold is priced in USD, exchange rate movements can affect demand and pricing.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://fred.stlouisfed.org/series/TWEXBGSMTH">FRED: TWEXBGSMTH</a>
      </td>
    </tr>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>Brent Crude Oil Price</strong> (<code>brent_price</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Global oil benchmark price (USD). Often used as a proxy for inflationary pressures and global demand conditions.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://fred.stlouisfed.org/series/POILBREUSDM">FRED: POILBREUSDM</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>MOVE Index</strong> (<code>MOVE_index</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Implied volatility in US Treasury markets. A proxy for bond market uncertainty and risk.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://uk.investing.com/indices/ice-bofaml-move-historical-data">Investing.com – ICE BofA MOVE</a>
      </td>
    </tr>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>MSCI World</strong> (<code>msci_world</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Equity performance across developed markets. Often interpreted as a proxy for global risk appetite.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://uk.investing.com/indices/msci-world-historical-data">Investing.com – MSCI World</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>MSCI Emerging Markets</strong> (<code>msci_emerging_markets</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Equity performance across emerging markets.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://uk.investing.com/indices/msci-emerging-markets-historical-data">Investing.com – MSCI EM</a>
      </td>
    </tr>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>S&amp;P GSCI</strong> (<code>sp_gsci</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Broad commodity index capturing global commodity price movements.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://uk.investing.com/indices/sp-gsci-commodity-total-return-historical-data">Investing.com – S&amp;P GSCI</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>Commodity Market Volatility</strong> (<code>commodity_equity_volatility</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        News-based measure of equity market volatility specific to commodity markets.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://fred.stlouisfed.org/series/EMVCOMMMKT">FRED: EMVCOMMMKT</a>
      </td>
    </tr>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>US Inflation Sentiment</strong> (<code>us_inflation_expectations</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Consumer survey-based measure of expected price developments in the United States.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://fred.stlouisfed.org/series/CSINFT02USM460S">FRED: CSINFT02USM460S</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>Euro Area Inflation Sentiment</strong> (<code>euro_area_inflation_expectations</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Consumer survey-based measure of expected price developments in the Euro Area.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://fred.stlouisfed.org/series/CSINFT02EZM460S">FRED: CSINFT02EZM460S</a>
      </td>
    </tr>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>World Trade Volume</strong> (<code>world_trade_volume</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Global merchandise trade index (fixed base 2021=100). Proxy for global demand conditions.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://www.cpb.nl/en/world-trade-monitor">CPB World Trade Monitor</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>World Industrial Production</strong> (<code>world_industrial_production</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Global industrial production index. Proxy for real economic activity.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://www.cpb.nl/en/world-trade-monitor">CPB World Trade Monitor</a>
      </td>
    </tr>
    <tr style="background-color:#ffffff;">
      <td style="padding:10px; border:1px solid #999;"><strong>Global Supply Chain Pressure Index</strong> (<code>gscpi</code>)</td>
      <td style="padding:10px; border:1px solid #999;">
        Composite index measuring global supply chain disruptions.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://www.newyorkfed.org/research/policy/gscpi#/overview">Federal Reserve Bank of New York – GSCPI</a>
      </td>
    </tr>
    <tr style="background-color:#fafafa;">
      <td style="padding:10px; border:1px solid #999;"><strong>National Financial Conditions Index</strong> (to construct)</td>
      <td style="padding:10px; border:1px solid #999;">
        Weekly index summarising credit conditions, leverage, and risk in US financial markets. Must be aggregated to monthly frequency.
      </td>
      <td style="padding:10px; border:1px solid #999;">
        <a href="https://www.chicagofed.org/research/data/nfci/current-data">Federal Reserve Bank of Chicago – NFCI</a>
      </td>
    </tr>
  </tbody>
</table>

### 1.3 Construction and Finalisation of the Dataset (5 marks)

#### 1.3.1 Construct the Target Variable

Let $P_t$ denote the gold price in month $t$.

Define the monthly return:

$$
r_t = 100 \times \frac{P_t - P_{t-1}}{P_{t-1}}
$$

Your prediction target is:

$$
r_{t+1}
$$

That is, the return realised in the month following the predictors.

##### Alignment in practice

Each row of your modelling dataset corresponds to month $t$.
The predictors observed in month $t$ are paired with the return realised in month $t+1$.

Example:

* January 2020 price = 1550
* February 2020 price = 1600

$$
r_{\text{Feb 2020}} = 100 \times \frac{1600 - 1550}{1550} = 3.23
$$

The row containing **January 2020 predictors** is associated with **3.23** (i.e with $r_{\text{Feb 2020}}$) as the outcome.

Construct this target variable and clearly verify that the alignment is correct.


#### 1.3.2 Construct Real Yield

Gold is frequently analysed relative to **real interest rates**, not nominal ones.
The real yield reflects the inflation-adjusted return on government bonds and captures the opportunity cost of holding a non-yielding asset like gold.

Construct the real yield as:

$$
\text{Real Yield}_t = \text{GS10}_t - \text{T10YIEM}_t
$$

Briefly explain why this variable may be economically relevant for gold prices.

#### 1.3.3 Integrate Financial Conditions

The NFCI dataset is observed at weekly frequency.

Aggregate the NFCI series to monthly frequency, merge it with the main dataset, and justify your aggregation decision.

#### 1.3.4 Dataset Assessment

Provide a concise assessment of your final modelling dataset:

* Time coverage
* Missing values
* Potential modelling implications

### 1.4 Data Exploration (10 marks)

Organise your code and markdown clearly.

Your exploration must include:

1. Plot the evolution of gold prices over time.
2. Construct and plot monthly gold returns.
3. Identify the five months with the largest absolute returns and comment briefly on possible economic context.
4. Compute correlations between gold returns and at least five predictors of your choice. Present them clearly (table or heatmap).
5. Produce at least one multi-variable visualisation involving gold returns and two predictors (e.g. colour, size, or faceting). Interpret what it suggests.

Your interpretation should focus on economic meaning and modelling implications.

### 1.5 Modelling (23 marks)

#### 1.5.1 Train/Test Split

Choose and justify a time-based train/test split appropriate for forecasting.

#### 1.5.2 Baseline Model

Build a baseline **linear regression model** to predict next-month gold returns.

Interpret its coefficients and evaluate its performance.
Justify your modelling and evaluation choices.


#### 1.5.3 Alternative Approach

Develop and evaluate an alternative modelling approach.

An alternative may involve:

* different feature engineering decisions (e.g., lags, transformations, scaling, interaction terms),
* a different regression model suitable for continuous outcomes,
* a different validation strategy within the training period.

The objective is not to maximise performance through extensive experimentation.
A small number of well-justified modelling decisions is preferable to many loosely motivated models.

Explain clearly:

* why the alternative approach was chosen,
* how it differs from the baseline,
* whether and why it improves (or does not improve) performance.


### 1.6 Discussion (12 marks)

Discuss:

* How predictable gold returns appear to be in your sample.
* Which predictors seem most economically meaningful.
* The limitations of your modelling strategy.
* What you would explore next if given additional time or data.

Your discussion should reflect on modelling decisions, uncertainty, and economic interpretation.


## Part 2: Predicting Sovereign Credit Ratings (50 marks)

Sovereign credit ratings reflect assessments of a country’s ability and willingness to meet its debt obligations. These ratings are issued by credit rating agencies such as Standard & Poor’s, Moody’s, and Fitch. While agencies may differ slightly in methodology, ratings broadly reflect macroeconomic performance, institutional quality, fiscal sustainability, and external vulnerability.

In this part, you will work with **Fitch sovereign ratings** and build models to predict whether a country will be classified as **Investment Grade (IG)** in the following year.

The dataset is structured as a country–year panel.

### 2.1 Data and Indicators


[![Download CSV](https://img.shields.io/badge/Download-sovereign_ratings_dataset_(csv_file)-b284be?style=for-the-badge&logo=download)](sovereign_ratings_data.csv)

The dataset merges:

* World Bank governance indicators
* World Bank macroeconomic indicators
* IMF World Economic Outlook data
* IMF Real Effective Exchange Rate data
* Fitch sovereign ratings

Each row corresponds to a **country–year** observation.

The indicators available are summarised below.

<table border="2">
<thead>
<tr>
<th><strong>Indicator (dataset variable)</strong></th>
<th><strong>Meaning</strong></th>
<th><strong>Source</strong></th>
</tr>
</thead>
<tbody>

<tr>
<td><strong>Sovereign Rating</strong> (<code>rating</code>)</td>
<td>
Letter rating assigned by Fitch (e.g. AAA, BBB, BB+, etc.). Ratings reflect the agency’s assessment of default risk.
</td>
<td>
<a href='https://ratingshistory.info/'>Fitch Ratings</a>
</td>
</tr>

<tr>
<td><strong>Control of Corruption</strong> (<code>CC.EST</code>)</td>
<td>
Perception of the extent to which public power is exercised for private gain. Higher values indicate better governance quality.
</td>
<td>
<a href="https://data.worldbank.org/indicator/CC.EST">World Bank – Worldwide Governance Indicators</a>
</td>
</tr>

<tr>
<td><strong>Government Effectiveness</strong> (<code>GE.EST</code>)</td>
<td>
Quality of public services and policy implementation.
</td>
<td>
<a href="https://data.worldbank.org/indicator/GE.EST">World Bank – Worldwide Governance Indicators</a>
</td>
</tr>

<tr>
<td><strong>Regulatory Quality</strong> (<code>RQ.EST</code>)</td>
<td>
Ability of the government to formulate and implement sound policies.
</td>
<td>
<a href="https://data.worldbank.org/indicator/RQ.EST">World Bank – Worldwide Governance Indicators</a>
</td>
</tr>

<tr>
<td><strong>Rule of Law</strong> (<code>RL.EST</code>)</td>
<td>
Confidence in contract enforcement and property rights.
</td>
<td>
<a href="https://data.worldbank.org/indicator/RL.EST">World Bank – Worldwide Governance Indicators</a>
</td>
</tr>

<tr>
<td><strong>GDP Growth</strong> (<code>NY.GDP.MKTP.KD.ZG</code>)</td>
<td>
Annual percentage growth rate of GDP at constant prices.
</td>
<td>
<a href="https://data.worldbank.org/indicator/NY.GDP.MKTP.KD.ZG">World Bank</a>
</td>
</tr>

<tr>
<td><strong>Current Account Balance (% GDP)</strong> (<code>BN.CAB.XOKA.GD.ZS</code>)</td>
<td>
Net exports plus net income and transfers, expressed as % of GDP.
</td>
<td>
<a href="https://data.worldbank.org/indicator/BN.CAB.XOKA.GD.ZS">World Bank</a>
</td>
</tr>

<tr>
<td><strong>Trade Openness (% GDP)</strong> (<code>NE.TRD.GNFS.ZS</code>)</td>
<td>
Sum of exports and imports as percentage of GDP.
</td>
<td>
<a href="https://data.worldbank.org/indicator/NE.TRD.GNFS.ZS">World Bank</a>
</td>
</tr>

<tr>
<td><strong>Gross Government Debt (% GDP)</strong> (<code>GGXWDG_NGDP</code>)</td>
<td>
General government gross debt as percentage of GDP.
</td>
<td>
<a href="https://www.imf.org/en/Publications/WEO">IMF World Economic Outlook</a>
</td>
</tr>

<tr>
<td><strong>Structural Balance (% GDP)</strong> (<code>GGSB_NPGDP</code>)</td>
<td>
Cyclically-adjusted fiscal balance as % of GDP.
</td>
<td>
<a href="https://www.imf.org/en/publications/sprolls/world-economic-outlook-databases">IMF World Economic Outlook</a>
</td>
</tr>

<tr>
<td><strong>Inflation</strong> (<code>PCPI</code>)</td>
<td>
Annual consumer price inflation (period average).
</td>
<td>
<a href="https://www.imf.org/en/publications/sprolls/world-economic-outlook-databases">IMF World Economic Outlook</a>
</td>
</tr>

<tr>
<td><strong>Real Effective Exchange Rate</strong> (<code>REER_IX_RY2010_ACW_RCPI</code>)</td>
<td>
Index measuring international competitiveness relative to trading partners.
</td>
<td>
<a href="https://www.imf.org/en/publications/sprolls/world-economic-outlook-databases">IMF REER Database</a>
</td>
</tr>

</tbody>
</table>


### 2.2 Outcome Construction and Panel Alignment (5 marks)

Fitch ratings are expressed as ordered letter grades. A sovereign is considered **Investment Grade (IG)** if its rating is **BBB− or above**.

**2.2.1** Construct a binary variable $is_{{ig}_t}$ indicating whether a country is investment grade in year *t*.

**2.2.2** Construct the forecasting target:

$$
is_{{ig}_{t+1}}
$$

Each country–year observation at time *t* must be paired with the IG status of the same country in year *t+1*.

**2.2.3** Clearly explain how you handled:

* countries without consecutive observations,
* countries entering or exiting the sample.

### 2.3 Data Exploration (10 marks)

**Q2.3.1** Examine the distribution of Fitch ratings across the sample.
How concentrated are ratings at the top or bottom of the scale?

**Q2.3.2** Identify rating switches over time:

* Which countries experienced rating upgrades or downgrades?
* How frequent are rating changes overall?

**Q2.3.3** Do all rating changes result in a change in Investment Grade status?
Provide examples and discuss.

**Q2.3.4** Compare average values of at least five macroeconomic indicators between IG and non-IG countries. Interpret the differences.

**Q2.3.5** Produce at least one multi-variable visualisation involving IG status and two predictors. Interpret it.


### 2.4 Modelling (23 marks)

#### Q2.4.1

Choose and justify a time-based train/test split.


#### Q2.4.2 Baseline model

Build a baseline **logistic regression model** to predict next-year Investment Grade status.

Interpret its coefficients and evaluate its performance.
Justify your modelling and evaluation choices.


#### Q2.4.3 Alternative approach

Develop and evaluate an alternative modelling approach.

Justify your modelling and evaluation choices.

The goal is not to maximise raw performance at all costs, but to demonstrate coherent reasoning in model construction, evaluation, and interpretation.


### 2.5 Discussion (12 marks)

Discuss:

* How predictable sovereign IG status appears to be.
* Whether macroeconomic variables alone seem sufficient to explain rating dynamics.
* The implications of treating panel observations as independent.
* Limitations of your modelling approach.
* What extensions (methodological or data-related) you would consider next.


>[!IMPORTANT]
>## Principles to bear in mind for all parts!
>1. We've seen many models until now and you might be tempted to try and show us every single model you know, in particular in the questions calling upon you to improve model performance. **Don't!** <br/>
Resist the siren calls🧜‍♀️ and make resolute model choices. Model selection is a skill! So, **DO NOT TRY EVERY SINGLE MODEL UNDER THE SUN** to tackle to the questions. State your modeling hypotheses clearly, justify your choices and only choose a couple of models to try and solve the questions.
>
>2. You are obviously allowed to use dimensionality reduction techniques e.g PCA/MCA/FAMD/UMAP (W07) if you think it might help with your modeling (again justify their use if you do use them!). But you don't have to use them. This summative is mainly about **supervised learning techniques**.
>
>3. Simply lining up code without explanation will not get you high grades. We expect you to justify your modeling choices (e.g why did you choose to use a particular model in the particular context of the problem you're solving? why is it uniquely suitable for the dataset/problem context? How did you set its parameters?) and to explain the model results and metrics in the context of the problem you're dealing with.

# ✔️ How we will grade your work

Following the instructions carefully and competently across both parts should result in an overall mark in the **60–69** range.
To obtain 70% or above, your work must demonstrate strong modelling judgement, correct handling of temporal structure, careful preprocessing, and clear interpretation. Only if you go above and beyond what is asked of you _in a meaningful way_ will you get scores of 70% or above. Simply adding more code^[Hint: don't just write code, especially uncommented chunks of code. It won't get you very far. Submissions consisting largely of code with little interpretation will receive a low mark, even if the code runs. You need to explain the code results, interpret them and put them in context.] or text will not get you a higher score; you need to add interesting insights or analyses to get a distinction.

⚠️ You will incur a penalty if you only submit a `.qmd` file and not also a properly rendered `.html` file alongside it! 

Following the instructions carefully and competently across both parts should result in an overall mark in the **30–34 range (per 50-mark part)** — i.e., around a low-to-mid 60 overall.

## Part 1: Gold Return Prediction (50 marks)

### **0–19 marks**

Serious fail.

This band includes work with one or more of the following:

* Incorrect construction of next-month returns.
* Incorrect construction of real yield.
* NFCI not aggregated properly or merged incorrectly.
* Clear data leakage (e.g., using future information in predictors).
* Incorrect or inappropriate train/test split (e.g., inappropriate split in time-series context).
* Baseline linear regression missing or fundamentally mis-specified.
* Inappropriate evaluation metrics for forecasting.
* No interpretation of coefficients.
* Submission mostly code with minimal explanation **even if technically correct**.
* Plots missing, unlabeled, or uninterpreted.
* Major formatting issues that hinder comprehension of the content

If the modelling design invalidates the exercise (e.g., leakage or incorrect target) or if we can't understand what you're trying to do, the mark will fall in this range.

### **20–24 marks**

Weak pass.

* Target and real yield constructed but with weaknesses or unclear alignment.
* Minor leakage risks or temporal inconsistencies.
* Train/test split present but poorly justified.
* Evaluation superficial or weakly justified.
* Coefficient interpretation incomplete or partially incorrect.
* Alternative approach minimal or not meaningfully distinct.
* Organisation or clarity issues.
* Noticeable formatting or organisation issues.

Demonstrates partial understanding but significant modelling weaknesses.

### **25–34 marks**

Solid pass to merit.

* Target, real yield, and NFCI correctly constructed.
* No serious leakage.
* Appropriate time-based train/test split.
* Baseline linear regression correctly specified.
* Evaluation metrics appropriate and justified.
* Coefficients interpreted correctly in economic terms.
* Alternative approach implemented and evaluated coherently.
* Minor preprocessing imperfections or limited depth of justification.
* Discussion addresses predictability and limitations, but not deeply.
* Plots labelled and interpreted.
* Interpretations could use more depth (e.g contextual information) or over-claim based on the evidence.

This band reflects **technically correct, coherent modelling**, but limited analytical depth or modelling sophistication.

### **35–39 marks**

Strong distinction-level work.

* Careful handling of temporal alignment and forecasting logic.
* Explicit awareness of leakage risks and modelling assumptions.
* Clean preprocessing and feature construction.
* Evaluation thoughtfully chosen and clearly justified.
* Coefficient interpretation precise and economically meaningful.
* Alternative modelling approach meaningfully different and well motivated.
* Discussion critically examines predictability and model limitations.
* Clear, well-structured presentation.

This band reflects **strong modelling judgement and analytical maturity** — not just correctness.

### **40–50 marks**

Exceptional work.

* No leakage, mis-specification, or alignment issues.
* Modelling design reflects deep understanding of forecasting constraints.
* Alternative approach adds genuine analytical value (not just a different algorithm).
* Evaluation demonstrates nuanced understanding of forecast difficulty.
* Interpretation shows insight into economic mechanisms and limitations.
* Discussion critically engages with model uncertainty and structural issues.
* Writing is precise, concise, and professional throughout.
* Evidence of model comparison reasoning grounded in forecasting theory rather than trial-and-error experimentation.

This band reflects **intellectual control of the modelling problem**, not merely strong technical execution.

Marks above 45 will be rare and reserved for work demonstrating exceptional analytical clarity and modelling discipline throughout.

## Part 2: Sovereign Ratings Classification (50 marks)

### **0–19 marks**

Serious fail.

Includes one or more of:

* Incorrect construction of investment-grade outcome.
* Misinterpretation of ratings transitions.
* Data leakage (e.g., using contemporaneous or future ratings in predictors).
* Incorrect handling of temporal structure.
* Logistic regression missing or fundamentally mis-specified.
* Inappropriate classification metrics.
* No interpretation of coefficients.
* Submission largely code without explanation.
* Plots missing, unlabeled, or uninterpreted.
* Major formatting issues that affect the comprehension of the content.

### **20–24 marks**

Weak pass.

* Investment-grade variable constructed but poorly explained.
* Some preprocessing or alignment weaknesses.
* Logistic regression implemented but weakly justified.
* Evaluation superficial or partially inappropriate.
* Coefficient interpretation limited or partially incorrect.
* Alternative approach weak or incoherent.
* Noticeable formatting or organisation issues.

Shows partial understanding but significant modelling weaknesses.

### **25–34 marks**

Solid pass to merit.

* Investment-grade target correctly constructed.
* No serious leakage.
* Logistic regression correctly specified.
* Appropriate classification metrics selected and justified.
* Coefficients interpreted correctly (log-odds and/or probability terms).
* Alternative modelling approach implemented and evaluated coherently.
* Minor modelling or justification weaknesses.
* Discussion addresses panel structure and limitations at a basic level.
* Plots labelled and interpreted.
* Interpretations could use more depth (e.g contextual information) or over-claim based on the evidence.

Technically correct and coherent, but without strong depth of modelling insight.

### **35–39 marks**

Strong distinction-level work.

* Careful treatment of temporal structure in panel setting.
* Clear awareness of independence assumptions and limitations.
* Thoughtful modelling design.
* Precise interpretation of logistic coefficients.
* Evaluation reflects understanding of imbalance and trade-offs.
* Alternative approach meaningfully distinct and justified.
* Discussion critically examines modelling assumptions and structural issues.
* Clear and professional presentation.

Reflects strong analytical judgement and modelling maturity.

### **40–50 marks**

Exceptional work.

* No leakage, mis-specification, or alignment errors.
* Clear understanding of prediction vs structural interpretation.
* Insightful handling of panel structure and modelling assumptions.
* Evaluation demonstrates nuanced understanding of classification trade-offs.
* Interpretation connects results meaningfully to economic reasoning.
* Discussion critically engages with rating dynamics and modelling limits.
* Writing precise, rigorous, and disciplined throughout.
* Clear distinction between predictive modelling and structural inference, with disciplined interpretation of results.

Marks above 45 will be rare and reserved for work demonstrating exceptional analytical clarity and modelling discipline throughout.


## 🙋 Getting help

You can post general coding questions on Slack but should not reveal code that is part of your solution. 

For example, you can ask:

- _"Does anyone know how I can create a logistic regression in `scikit-learn` with a `Pipeline`?"_
- _"Has anyone figured out how to do time-aware cross-validation??"_
- _"I tried using something like `pd.query("Date>'1997-05-06'")` but then I got an error "_ ([Reproducible example](https://stackoverflow.com/help/minimal-reproducible-example))
- _"Does anyone know how I can create a new variable that is the sum of two other variables?"_

You are allowed to share 'aesthetic' elements of your code if they are not part of the core of the solution. For example, suppose you find a really cool new way to generate a plot. You can share the code for the plot, using a generic `df` as the data frame, but you should not share the code for the data wrangling that led to the creation of `df`.

If we find that you posted something on Slack that violates this principle without realising it, you won't be penalised for it - don't worry, but we will delete your message and let you know.

## 👯 Collaborating with others

You are allowed to discuss the assignment with others, work alongside each other, and help each other. However, you cannot share or copy code from others — pretty much the same rules as above. You should also be careful about having distinct analytical pipelines.

## 🤖 Using AI help?

You can use Generative AI tools such as ChatGPT when doing this research and search online for help. If you use it, however minimal use you made, you are asked to report the AI tool you used and add an extra section to your notebook to explain how much you used it.

Note that while these tools can be helpful, they tend to generate responses that sound convincing but are not necessarily correct. Another problem is that they tend to create formulaic and repetitive responses, thus limiting your chances of getting a high mark. When it comes to coding, these tools tend to generate code that is not very efficient or old and does not follow the principles we teach in this course.

To see examples of how to report the use of AI tools, see 🤖 [Our Generative AI policy](https://lse-dsi.github.io/DS202/2025-2026/winter-term/generative-ai.html).



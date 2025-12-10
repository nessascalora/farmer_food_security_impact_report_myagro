myAgro Food Security Impact Analysis
==
#### Nessa Scalora, Data Scientist
##### November, 2025

# Contents

[Introduction](#Introduction)

[Study Design & Data Collection](#Study-Design-&-Data-Collection)

[Measures of Food Security](#Measures-of-Food-Security)

[Methodology](#Methodology)

[Results](#Results)

# Introduction

[myAgro's](https://www.myagro.org/) mission is to move West African smallholder farmers out of poverty. By improving farm yields and incomes, myAgro strengthens household food security—one of several outcomes in its Theory of Change. **This impact analysis tests whether myAgro households are indeed more food secure as a result of myAgro services.**

# Study Design & Data Collection

## Context

In rural Mali and Senegal, there is typically one main agricultural season each year. Farmers sow their fields with the onset of the five-month rainy season in June and begin harvesting in October. Food security follows this cycle: it peaks between October and January, when harvests are plentiful, and gradually declines as food stocks and monetary resources dwindle. The most difficult period, known as the "lean" or "hunger" season, falls between June and September, when supplies from the previous harvest are at their lowest.

## Hypotheses

1. Planting myAgro packages leads to improved household food security
    1. Throughout the year
    2. In the lean season
    3. Within each individual data collection period (1.5 months on average).
2. Planting larger packages leads to improved household food security
3. Planting higher-impact* myAgro packages leads to improved household food security

Where "improved food security" means a significantly *lower* Reduced Coping Strategy Index (rCSI) score among myAgro farmers compared to control farmers.

\*Impact of individual crop types are evaluated annually through myAgro's harvest measurement activity and subsequent impact calculations.

## Data Collection

11,854 food security surveys were conducted from a sample of control and treatment households in eight data collection periods from October 2023 until September 2024. This year-long period captures the full food security cycle that reflects the 2023 harvest. Each country had three household cohorts, with 771 to 801 households surveyed from about 40 villages at a time, for a total of 4,731 participating households in 245 villages across both treatment arms. A new cohort of households was selected every 3-4 months to avoid the potential bias and measurement error resulting from researcher and respondent fatigue. Each sample household was surveyed once per data collection period.

## Sample Methodology

The sample is stratified by country, with one strata in Mali and one in Senegal. Technically, stratifying increases the statistical power of the study and can improve the precision of results. However, the sample in each country is limited to one chosen research area due to logistical constraints. Sample villages were selected across the geographically clustered zones Lobougoula, Niena, Koumantou, and Kadiolo in Mali and the Passi, Ndoffane, Kaolack, Gossas, and Kaffrine in Senegal. **Therefore, the conclusions drawn are limited to the research areas only, and do not reflect all areas of myAgro operation across each country. This is important to disclose in results reporting.**

The sample is clustered by village. Clustering limits spillover effects, however, it increases standard error (variance), which leads to lower statistical significance (the distribution of data is more spread out for both the treatment and control groups, therefore a higher likelihood that they overlap). The village selection strategy attempts to balance logistical practicality and statistical power.

### Sample Sizes

**Sample size per country:** 400 households

**Number of villages per country:** 20 villages per treatment arm (40 total villages)

### Treatment Sample Selection

**Sample frame:** All qualifying farmers in qualifying villages in the client database.

**Qualifying villages:** Villages in the research area zones, excluding villages that had already participated in previous data collection periods, and that *have at least ten qualifying clients.*

**Qualifying clients:** Clients who have been delivered one or more core season packages in 2023.

**Procedure (for each country):**
1. Calculate the sample size for each zone (the proportion of the country sample size within each zone) using the density of qualifying farmers within each zone, so that zones with more farmers have larger representation within the sample.
2. Get sample villages: Randomly select 20 qualifying villages per zone from the sample frame.
    - Requirement: The total number of qualifying clients in the selected villages of the zone is greater than or equal to 150% the zone sample size. The buffer of farmers in selected villages helps minimize the need to add more villages after agents receive their village assignments, since adding more farmers is inevitable. The initial sample selected is not the final sample because about 30% of the farmers do not pass the in-person eligibility checks (requirements below), and are removed and replaced. We therefore ensure a large buffer of clients in the initially selected villages. (This condition is typically fulfilled faster than the village sample size is reached.)
3. Get the initial farmer sample: Randomly select farmers from the pool of qualifying clients across all sample villages until the zone sample sizes are met.
    - Requirement: At least five farmers are selected for the sample in each village to help minimize the travel required of field agents.

### Control Sample Selection

**Qualifying villages:** Villages in the research area zones in which myAgro does not currently operate, has not previously operated (in at least five years), and is at least 2 km away from the closest myAgro village (to avoid spillover effect).

**Qualifying farmers:** See eligibility requirements below.

**Procedure (for each country):**
1. Qualifying control villages are identified by the field team.
2. 20 control households per village are selected by survey agents in the field using the UNICEF pencil spin method that is suggested in the [Coping Strategy Index Field Methods Manual](https://www.indikit.net/document/9-the-coping-strategies-index-field-methods-manual) and outlined in the agent training materials.

### Eligibility Requirements for Household Participation (evaluated in-person by agents)

1. The household was consenting
2. Households are represented only once in the data (one respondent/participant per individual household)
3. myAgro client information corresponded to the information in the database
4. myAgro clients confirmed they were delivered in the most recent core season

### Missing Sample Controls

As established above, the eligibility criteria ensure that each household is represented as a single observation within the dataset. Although the analytical framework requires one observation per household for statistical independence, the magnitude of the treatment effect is positively correlated with the number of myAgro program participants within a given household, as cumulative myAgro packages contribute to enhanced household food security outcomes. Current data limitations preclude household identification for individual farmers, thereby restricting the assessment of treatment intensity to the sales data associated with the designated household representative. Future data collection protocols should incorporate comprehensive household roster information, including registration of all myAgro participants per household, to enable accurate quantification of aggregate treatment exposure at the household level.

### Assumptions

1. Participating myAgro clients used all the inputs they were delivered on their farms in the 2023 planting season, and on the recommended area.
2. There are no inherent, unseen differences between two villages in the same area that would lead to one village's participation in the program and not the other's.
3. Given the set of observed farmer characteristics controlled in the following analysis, the treatment assignment is independent of the potential outcomes.

# Food Security Metric: rCSI

**[Reduced Coping Strategies Index (rCSI):](https://www.indikit.net/document/9-the-coping-strategies-index-field-methods-manual)** Measures the frequency and severity of short-term behavioral strategies a household uses when it cannot access enough food or money to buy food. A higher score indicates more coping, and therefore higher food insecurity.

**We use rCSI to represent farmer food security levels because it:**
1. Captures an overall picture of food access, quality, and preferences
2. Is adequately sensitive for the study population and to [seasonality](https://whh.indikit.net/indicator/925-food-security/4847-rcsi-reduced-coping-strategy-index)
3. [Is appropriate for measuring the impact of long-term interventions](https://whh.indikit.net/indicator/925-food-security/4847-rcsi-reduced-coping-strategy-index)

## Components

EN: During the last 7 days, were there days (and, if so, how many) when your household had to employ one of the
    following strategies (to cope with a lack of food or money to buy it)?

FR: Pendant les 7 derniers jours, y a-t-il eu des jours (et si oui, combien) où votre ménage a dû employer une des
    stratégies suivantes pour faire face à un manque de nourriture ou d'argent pour en acheter?

### 'rcsi_borrow':
- EN: Borrowed food or relied on help from friends or relatives
- FR: Emprunter des vivres ou solliciter l'aide d'un ami ou d'un parent
- Weight: 2

### 'rcsi_limit':
- EN: Reduced portion size of meals
- FR: Limiter la taille des parts pendant les repas
- Weight: 1

### 'rcsi_reduce':
- EN: Reduced the number of meals eaten per day
- FR: Diminuer le nombre de repas par jour
- Weight: 1

### 'rcsi_rely':
- EN: Relied on less preferred, less expensive food
- FR: Recourir à des aliments moins appréciés et moins chers
- Weight: 1

### 'rcsi_restrict':
- EN: Restricted consumption by adults in order for small children to eat
- FR: Réduire les quantités consommés par les adultes /mères pour nourrir les enfants
- Weight: 3

## Calculation

**The weighted sum of the five components**

rCSI score range: 0-56

## Severity Categories

[Integrated Food Security Phase Classification (IPC)](https://www.ipcinfo.org/ipcinfo-website/ipc-overview-and-classification-system/en/) is a classification framework used to determine the severity and extent of acute and chronic food insecurity and acute malnutrition situations within countries, according to internationally recognized standards. [rCSI categories can be defined and aligned with IPC Phases as follows:](https://whh.indikit.net/indicator/925-food-security/4847-rcsi-reduced-coping-strategy-index)


| IPC Phase | Category | rCSI Score Range |
|---|:---:|---:|
| 1 | No to minimal food insecurity | 0-3 |
| 2 | "Stressed" phase; some food insecurity | 4-18 |
| 3 | Severe or crisis food insecurity | 19-56 |

# Methodology

The goal of this analysis is to ultimately understand the causal effect of myAgro intervention on household food security. We will do this by simulating randomized conditions in the data by controlling for covariates. As our treatment households are not randomly selected, and rather self-selected given the opportunity (depending on village program participation), we will use modeling techniques to eliminate the resulting selection bias so that we can directly compare the treatment and control groups.

We will get results on three levels relating to time:
1. Year-round (October 2023-September 2024)
2. Lean season (June-September 2024)
3. Data collection period (eight within the twelve months, each representing about one and a half months)

We will use LMMs to estimate ATE of individual treatments on the first two levels and inverse probability of treatment weighting (IPTW) to compare the weighted mean rCSI across treatments between groups on the third level.

## Linear Mixed-Effects Model (LMM)

A LMM is a statistical model used to analyze data where observations are not independent, such as repeated measurements or clustered data. LMM is an extension of standard linear regression that includes both fixed effects and random effects. **We use LMM to estimate year-round and lean season Average Treatment Effects (ATE) on household food security for each myAgro crop type planted in the most recent season and cumulative prior-season participation, capturing both recent harvest impacts and the longer-term effects of sustained program engagement.**

Similar studies that must control for selection bias between the treatment and control groups typically use matching techniques to estimate the ATE of an intervention. However, our study requires a different methodology for several reasons:
1. The nutrition survey data is hierarchical in nature, with dimensions like time of year, geographic location, and individual household. There are 3-4 surveys per household that capture their food security in different data collection periods. Therefore, each survey response is not a fully independent observation, and this is required for matching.
2. The study encompasses several treatment variables, since myAgro participation isn't technically binary--sample clients planted a variety of packages (seeds, fertilizer, and other agricultural inputs of different crop types and quantities, where quantity represents the area of land that the inputs cover in hectares). Matching techniques are restricted to estimating ATE for studies simply comparing an outcome variable between treatment and control groups.
3. The ideal way to properly control for covariates in our study is to use propensity score (probability of treatment) as a covariate. It reduces the covariates related to household info--poverty level, size of farm, and main crop type(s) cultivated--into one variable to include in the model.
4. Furthermore, our data has many subgroups of farmers considering all the variables we are interested in. Some of these groups are small, but we still care about them. The LMM handles sparsity better than matching because matching treats observations in small groups as outliers.

### Food Security Model

#### Data Hierarchy

**Nesting:** household ⊂ village ⊂ cohort ⊂ country


**Repeated measures:** 3-4 surveys per household in different time periods

#### Fixed Effects

1. **Country**: Mali or Senegal (one-hot encoded)
2. **Cohort**: household cohorts 1, 2, and 3 (one-hot encoded)
3. **Propensity**: The probability (0-1) that a household is selected for treatment
    - Propensity score was calculated using an XGBoost algorithm with a T-learned meta-learner with the following features:
        - [Poverty Probability Index (PPI)](https://www.povertyindex.org/home): household poverty level proxy (continuous)
        - Total land cultivated (hectares): Total acres farmed (continuous)
        - Main crop type cultivated (one-hot encoded; 13 features)
5. **sin_t & cos_t**: Cyclical time variables created from data collection period to capture the seasonality of food security (data collection period) (continuous)
6. **All treatment variables** (continuous)

##### Time & Seasonality

Because we have one full seasonal cycle, we will use sin/cos seasonal terms to capture smooth annual variation, plus a linear term for secular trend. All from from **data collection period:**
1. sin_t
2. cis_t
3. t_c (t - mean(t))

##### t_c: A centered version of the time variable (data collection period)

Why center it:
- In mixed models, random intercepts and random slopes can be highly correlated if time is not centered.
- Centering improves numerical stability and makes the intercept interpretable:
    - Without centering: intercept = predicted food security at t = 0 (first data collection period).
    - With centering: intercept = predicted rCSI at average month in the data.
- Random slope: (1 + t_c | household) → each household can have its own linear trend over time.
    - **Centering ensures the intercept represents the household's average rCSI, not the value at the first month.**
- Fixed effect: t_c captures overall linear change over the year (on top of seasonal sin/cos).

##### Treatment Variables

There are 11 variables included as fixed effects that capture myAgro intervention as treatment.
- **2023 treatment by product:** Nine continuous variables that each represent the treatment level of a single myAgro product, i.e the number of hectares delivered per product in the 2023 core season.
    - cowpea
    - maize
    - millet
    - okra
    - peanut
    - rice
    - roselle
    - sorghum
    - watermelon

- **Past treatment:** A continuous variable that represents the number of hectares delivered of any product in any season before 2023. This captures the isolated impact of sustained myAgro participation over multiple seasons on household food security, independent from the impact of the most recent harvest.

- **25kg fertilizer:** A binary variable representing clients that received the 25kg fertilizer gift sponsored by the ASAA program in 2023. All farmers in Mali who were delivered a core package received this extra fertilizer.
    - **Note:** Since all Mali households are True for the 25kg fertilizer treatment variable (and all Senegal households are False), there is an interaction between the fertilizer treatment variable and the main effects of the other treatments.

#### Random Effects

The random intercept + slope captures the repeated measures and allows households to vary in seasonal response. Households differ in how rCSI changes over time.

**Random intercept:** Household ID

**Random slope:** Time (centered data collection period)

**Not Used: Village Variance Component**

We initially considered including a village-level variance component in our random effects structure to account for potential clustering at the village level. However, this specification resulted in model convergence issues, with the optimizer unable to cleanly partition variance between household-level slopes and village-level clusters. Even when we simplified the structure by including only a village random intercept (without random slopes), the variance component consistently collapsed to near-zero, indicating that village-level clustering was either minimal or already captured by the household-level random effects. The singular fit warnings confirmed that the village variance component was not well-identified and represented an overparameterization of the random effects structure. Given that households are nested within villages, the household random intercepts were already absorbing any meaningful village-level variation, making the additional village component redundant. Therefore, our final model specification included only household ID random intercepts and centered time random slopes, which provided a parsimonious structure that captured the relevant variance components while maintaining model stability and convergence.

## IPTW Weighted Average rCSI

We use average rCSI score, weighted by the inverse of treatment probability (inverse of propensity score), to visualize and compare the food security outcomes of both treatment and control groups by individual data collection period.

We cannot use modeling techniques to achieve this because model coefficients give us the controlled *difference* in outcomes between groups, not the outcomes themselves. IPTW allows us to get average rCSI scores and still control for the covariates captured by the propensity score (poverty level, farm size, main crop type(s) cultivated). Additionally, unlike matching, it allows us to keep all of our observations.

However, there are several disadvantage of the IPTW approach compared to LMMs:
1. We must use a binary treatment variable--treatment or control--instead of the 11 continuous variables used in the LMM. Therefore, the results will reflect the general impact of myAgro intervention, not of its individual products or their treatment levels (hectares).
2. The hierarchal nature of the data is not captured by specifying fixed and random effects.

In reporting, these caveats must be clearly communicated, and the results must be interpreted as a supplement beside the model results.

### Formulas

We calculate the weighted average rCSI for each treatment arm, as well as the ATE, for each of eight data collection periods using the following formulas.

The absence of extreme propensity score values (approaching 0 or 1) in both treatment arms indicates that weight stabilization is unnecessary. Stabilization is typically employed when extreme weights inflate variance and increase outcome sensitivity to outliers, conditions not present in our sample.

#### Weights Definition
For each observation $i$:

$$w_i = \begin{cases}
\frac{1}{p_i} & \text{if } T_i = 1 \text{ (treatment)} \\
\frac{1}{1-p_i} & \text{if } T_i = 0 \text{ (control)}
\end{cases}$$

Where:
- $p_i$ = propensity score for observation $i$
- $T_i$ = treatment indicator (1 = treatment, 0 = control)

#### Weighted Average for Each Group

**Treatment Group:**

$$\bar{Y}_1^w = \frac{\sum_{i=1}^{n} w_i \cdot \text{rcsi}_i \cdot T_i}{\sum_{i=1}^{n} w_i \cdot T_i}$$

**Control Group:**

$$\bar{Y}_0^w = \frac{\sum_{i=1}^{n} w_i \cdot \text{rcsi}_i \cdot (1-T_i)}{\sum_{i=1}^{n} w_i \cdot (1-T_i)}$$

#### Average Treatment Effect
The weighted average treatment effect would then be:
$$\text{ATE}^w = \bar{Y}_1^w - \bar{Y}_0^w$$

# Results

See the final report document "myAgro Food Security Impact Report November 2025" for final results.

# Repository Structure

```
food_security_impact_report/
├── README.md                              # This file
├── food_security_impact_analysis.ipynb    # Analysis notebook
├── survey_data_clean_anonymized.csv       # Cleaned survey data
├── requirements.txt                       # Python dependencies
├── LICENSE                                # License file
└── .gitignore                             # Git ignore file
```

# Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/food_security_impact_report.git
cd food_security_impact_report
```

2. Create a virtual environment (recommended):
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

# Usage

Open and run the Jupyter notebook:
```bash
jupyter notebook food_security_impact_analysis.ipynb
```

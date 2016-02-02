## 3.3 CHAT Data Analysis Tip Sheet

The following summarized some PSG variables of likely interest to CHAT investigators:

### 3.3.1 Summary of interesting PSG Variables

| Name                                            |     |  Category     |     #  |  Description                               |
|:------------------------------------------------|:---:|:--------------|-------:|:-------------------------------------------|
|  [slp_eff](https://sleepdata.org/datasets/chat/variables/slp_eff)        |  1  |  Time         |  1371  |  Filtered: Sleep efficiency %              |
|  [timest1p](https://sleepdata.org/datasets/chat/variables/timest1p)      |  1  |  Stages       |  1372  |  Filtered: % time stage 1                  |
|  [timest1](https://sleepdata.org/datasets/chat/variables/timest1)        |  1  |  Stages       |  1373  |  Filtered: Time stage 1 (minutes)          |
|  [timest2p](https://sleepdata.org/datasets/chat/variables/timest2p)      |  1  |  Stages       |  1374  |  Filtered: % time stage 2                  |
|  [timest2](https://sleepdata.org/datasets/chat/variables/timest2)        |  1  |  Stages       |  1375  |  Filtered: Time stage 2 (minutes)          |
|  [times34p](https://sleepdata.org/datasets/chat/variables/times34p)      |  1  |  Stages       |  1376  |  Filtered: % time stage 3-4                |
|  [timest34](https://sleepdata.org/datasets/chat/variables/timest34)      |  1  |  Stages       |  1377  |  Filtered: Time stage 3-4 (minutes)        |
|  [timeremp](https://sleepdata.org/datasets/chat/variables/timeremp)      |  1  |  Stages       |  1378  |  Filtered: % time REM                      |
|  [BPMAVG](https://sleepdata.org/datasets/chat/variables/bpmavg)          |  1  |  Heart Rate   |  172   |  PSG Report: Average Heart rate (bpm)      |
|  [omahi3](https://sleepdata.org/datasets/chat/variables/omahi3)          |  1  |  Respiratory  |  1418  |  Filtered: CHAT AHI <br /> (Obstructive apneas all desats, Mixed apneas all desats, plus hypopneas with 3% or arousal) no centrals  |
|  [omai0p](https://sleepdata.org/datasets/chat/variables/omai0p)          |  1  |  Respiratory  |  1422  |  Filtered: CHAT OAI (Obstructive/Mixed Apnea Index all desats) no centrals  |
|  [cai0p](https://sleepdata.org/datasets/chat/variables/cai0p)            |  1  |  Respiratory  |  1425  |  Filtered: Central Apnea Index all desats  |
|  [avgsat](https://sleepdata.org/datasets/chat/variables/avgsat)          |     |  Oxygen       |  1443  |  Filtered: Average SaO2 in sleep           |
|  [minsat](https://sleepdata.org/datasets/chat/variables/minsat)          |     |  Oxygen       |  1444  |  Filtered: Minimum SaO2 in sleep           |
|  [AVGPLM](https://sleepdata.org/datasets/chat/variables/avgplm)          |  1  |  Legs         |  1025  |  PSG Report: # of PLM per hour of sleep    |
|  [rCO2PEAK](https://sleepdata.org/datasets/chat/variables/rco2peak)      |  1  |  CO2          |  1445  |  Filtered: Peak EtCO2 Asleep Restricted to QuCap = 3, 4, 5 PSG Report: Peak EtCO2 Asleep  |
|  [rPCTCO2G45](https://sleepdata.org/datasets/chat/variables/rpctco2g45)  |  1  |  CO2          |  1450  |  Filtered: % total sleep time EtCO2 > 45 mmHg  Restricted to QuCap = 3, 4, 5 PSG Report: % total sleep time EtCO2 > 45 mmHg  |
|  [rPCTCO2G50](https://sleepdata.org/datasets/chat/variables/rpctco2g50)  |  1  |  CO2          |  1451  |  Filtered: % total sleep time EtCO2 > 50 mmHg  Restricted to QuCap = 3, 4, 5 PSG Report: % total sleep time EtCO2 > 50 mmHg  |
|  [pctle92](https://sleepdata.org/datasets/chat/variables/pctle92)        |  1  |  Oxygen       |  1433  |  Filtered : % sleep time SaO2 is <= 92%  Restrict QuOxim = 3, 4, 5 Percent of sleep time with oxygen saturation <= 92%  [100*(Total Number of minutes with SaO2 <= 92) / (total sleep time)].  |
|  [ai_all](https://sleepdata.org/datasets/chat/variables/ai_all)          |  1  |  Arousals     |  1383  |  Filtered: Overall Arousal Index           |
|  [omahi3nr](https://sleepdata.org/datasets/chat/variables/omahi3nr)      |  1  |  Respiratory  |  1456  |  Filtered: Non-REM CHAT AHI (Obstructive apneas all desats, Mixed apneas all desats, plus hypopneas with 3% or arousal)  |
|  [omahi3r](https://sleepdata.org/datasets/chat/variables/omahi3r)        |  1  |  Respiratory  |  1455  |  Filtered: REM CHAT AHI (Obstructive apneas all desats, Mixed apneas all desats, plus hypopneas with 3% or arousal)  |
|  [omahi3b](https://sleepdata.org/datasets/chat/variables/omahi3b)        |  1  |  Respiratory  |  1457  |  Filtered: Supine CHAT AHI (Obstructive apneas all desats, Mixed apneas all desats, plus hypopneas with 3% or arousal)  |
|  [omahi3o](https://sleepdata.org/datasets/chat/variables/omahi3o)        |  1  |  Respiratory  |  1458  |  Filtered: Non-Supine CHAT AHI (Obstructive apneas all desats, Mixed apneas all desats, plus hypopneas with 3% or arousal)  |


### 3.3.2 Suggestions, Transformations, and Derivations of Key Variables

<div class="bs-callout bs-callout-info">
  <p>
    Note that some of the discussion items were developed by the Sleep Heart Health Study, with special credit to HL Kichner and E Shahar.
  </p>
</div>

A number of key sleep-related variables are not normally distributed.  Modeling these variables as the dependent variables violates assumptions of linear regression.  Achieving normality, or identifying alternative methods to use these data is important not only for consistency across publications, but also for accurate reporting of results.

The following PSG variables appear reasonably normally distributed and usually can be analyzed without transformations:  Sleep Stage 2, Sleep Stage REM, BPMAVG, CO2PEAK

The following are non-normal but can be achieve approximate normal distributions with a natural log transform (adding 0.010): Sleep Efficiency, OAHI, OAMHI, avgsat, minsat.

The following are highly skewed and cannot be easily transformed. Using categorical values may be necessary for any statistics sensitive to non-normality: Central Apnea Index; PCTCO2G45, PCTCO2G50, avgPLM

**AHI Values:** A number of AHI/RDI variables exist in the data set. These variables are highly skewed, with many people having small values and relatively few with very large values.  When AHI/RDI is the dependent variable log-transformation is recommended.  Since RDI=0 cannot be log-transformed, one should add some constant.  Key questions are: what value should the constant take? Should the constant be added to every RDI value or just to RDI=0? It turns out that slightly different answers to these seemingly minor questions could have non-trivial effects on the result.

**Central Apnea Index (CAI):**  Several variables describe central breathing events, with different thresholds for desaturation and requirement/non-requirement of arousals.  Central events are uncommon, with many subjects having zero values. Thus, when central events are of interest, may want to dichotomize these variables.  May consider dichotomizing at a CAI >1 which identifies approximately the highest 25%ile.

**Sleep Stages:** These data are reported in the data set as integers. Stage 1 and stage 3 – 4 are not normally distributed, but stage 2 and REM sleep are. (NOTE: since the data are integers, values must be divided by 100 prior to transformation to yield proportions).

**Sleep time below 92% O2:** Since a considerable proportion of the cohort had zero values, may need to dichotomize this variable (e.g., any time below 92%-identifying about top 5% of values).

**A General Note:** Back-transformation of the difference between two means of a log-transformed variable generates the geometric mean ratio (which is, more or less, the ratio of two medians). Not so for log-log transformation.

**Independent Continuous Predictors:**

The AHI/RDI and other sleep variables are often key predictors, rather than dependent variables. In such cases, log transformation is not needed but the challenge is even greater:  How to model those variables appropriately?  Three general approaches are commonly used (not necessarily mutually exclusive).  For each approach, we mention below key issues that ought to be considered.

<u>Paradigm 1:</u>  Statistical hypothesis testing. Fit the variable as is (continuous), test the null on its coefficient. If significant, fit a quadratic term as well.  If NOT significant, conclude a linear relation (or log-linear if using a log-linear model).

Drawbacks:

- There is a clear trend to minimize the use of P-values in statistical inference.
- A straight line and parabola are not the only possible shapes of the dose-response function in the data

<u>Paradigm 2:</u>  Categorical analysis.  Categorize the variable.  Issues:  how many categories?  Where to place the cutoff values?  A key consideration is having “enough data” within each category.  Some people prefer “clinical cutpoint” but sometimes the argument is circular since clinical cutpoints are (or should be) based on research findings.

Drawbacks:

- Results could be strongly dependent on the location of cutoff points.
- Tail effects are sometimes hidden (collapsed into an average effect of the last category)
- Categorical analysis is often followed by a “test for trend” which is erroneously interpreted as a test for monotonic dose-response. It is not.
- The risk function is forced to behave as a step-function

<u>Paradigm 3:</u>  Non-parametric or semi-parametric dose-response functions. Not as sensitive to location of cutoff points. Fewer model-imposed restriction. Visual display of the dose-response function.

Drawbacks:

- A bit more complicated to fit (though not much)
- No “concise” list of point estimates (though can be read off the graph)
- Other (beyond the scope of this document)


<hr class="soften" style="margin-top: 20px;margin-bottom: 20px;"/>

<div class="center">
<div class="btn-group">
  <a href=":pages_path:/psg-data-guide/3-20-condensed-data-dictionary.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-left"></span>
    3.2 Condensed Data Dictionary
  </a>

  <a href=":pages_path:/psg-data-guide/3-00-psg-data-guide-toc.md" class="btn btn-default">
    <span class="glyphicon glyphicon-chevron-up"></span>
    PSG Data Guide
  </a>
</div>
</div>

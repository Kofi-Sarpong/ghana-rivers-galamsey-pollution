# Methodology & Technical Documentation
## Ghana's Rivers in Crisis — Galamsey Pollution Dashboard

## Project Overview

Galamsey and other mining activities can affect water resources through
the introduction of metals and changes in water chemistry. This project
analyzes available water-quality measurements to identify where sampled
rivers exceed selected safety limits, determine the severity and
distribution of contaminant exceedances, and translate the findings into
potential response strategies.

The project follows this analytical progression:

**Where is the problem? → What is contaminating the water? → How severe
is it? → What can be done?**

------------------------------------------------------------------------

##  Objectives

-   Identify sampled rivers with contaminant levels above the applicable
    Ghana Standard limits.
-   Examine the distribution of arsenic, cadmium, chromium, and lead
    exceedances.
-   Measure contamination severity using exceedance ratios and
    exceedance-based measures.
-   Assess river-water pH against the recommended safe range.
-   Identify contaminants contributing most to the overall contamination
    burden.
-   Present the geographic distribution of sampled rivers across Ghana.
-   Translate analytical findings into short-, medium-, and long-term
    response strategies.

------------------------------------------------------------------------

##  Dataset

### Data Source

**Open Data Bank Ghana**

The dataset contains water-quality measurements from selected rivers and
a galamsey mining-site sample in Ghana.

### Samples

-   **11 river samples**
-   **1 Galamsey Pit sample**

The Galamsey Pit is treated separately from the rivers because it
represents a mining-site sample rather than a river.

### Parameters

-   Arsenic (As)
-   Cadmium (Cd)
-   Chromium (Cr)
-   Lead (Pb)
-   pH
-   Total Dissolved Solids (TDS)
-   Conductivity
-   Hardness
-   Calcium Hardness
-   Magnesium Hardness

The primary contaminant-exceedance analysis focuses on **As, Cd, Cr and
Pb**, together with **pH**.

------------------------------------------------------------------------

##  Analytical Methodology

### Ghana Standard as the Primary Benchmark

The **Ghana Standard** was used as the primary benchmark.

  Parameter         Ghana Standard
  --------------- ----------------
  Arsenic (As)           0.01 mg/L
  Cadmium (Cd)          0.003 mg/L
  Chromium (Cr)          0.05 mg/L
  Lead (Pb)              0.01 mg/L
  pH                      6.5--8.5

TDS and conductivity were also incorporated into the dashboard's
exceedance logic where applicable.

### Exceedance Ratio

**Exceedance Ratio = Sample Value ÷ Standard Limit**

An exceedance ratio of 44.4 means the observed concentration is 44.4
times the applicable standard limit.

Values at or below the applicable contaminant limit are represented as
zero in the contaminant-specific exceedance-ratio measures.

### Total Exceedance Index

The dashboard combines contaminant-specific exceedance ratios for:

-   Arsenic
-   Cadmium
-   Chromium
-   Lead

to create a **Total Exceedance Index** for comparing contamination
across river samples.

### Exceedance Amount

**Exceedance Amount = Sample Value − Standard Limit**

The measure is applied when the observed value exceeds the applicable
standard.

### Contamination Load

The dashboard aggregates exceedance amounts by contaminant to determine
the relative contribution of each contaminant to the overall
contamination load.

### Unsafe Rivers

A river is classified as having an exceedance when at least one of the
defined contaminant or pH criteria exceeds the applicable threshold.

**Unsafe Rivers (%) = Rivers with at least one exceedance ÷ Total Rivers
× 100**

### pH Assessment

pH is assessed against the recommended range of **6.5--8.5**.

------------------------------------------------------------------------

#  Dashboard

The dashboard contains **three pages**.

## 1. Rivers Overview

The first page provides the geographic and overall contamination
picture.

### Key components

-   **Map of Ghana** showing sampled rivers and their regions.
-   **Total Rivers** indicator.
-   **Unsafe Rivers (%)** indicator.
-   **Highest Contaminant Load** indicator.
-   **Top 5 Most Contaminated Rivers** based on the Total Exceedance
    Index.

### Key question

> **Where is the problem, and what is the overall scale and severity of
> contamination?**

![Rivers Overview Dashboard](images/rivers-overview.png)

------------------------------------------------------------------------

## 2. Contaminants Breakdown

This page provides a detailed examination of contaminant distribution
and severity.

### Questions answered

  -----------------------------------------------------------------------
  Question                            Dashboard analysis
  ----------------------------------- -----------------------------------
  How many rivers contain each        Number of sampled rivers exceeding
  contaminant?                        the applicable limit

  Which contaminants exceeded safe    River-by-river contaminant
  limits in each river?               comparison

  What is the severity and spread of  Exceedance-ratio analysis
  exceedances?                        

  Which contaminant exceeded the safe Contamination-load contribution
  limit by the widest margin?         

  How do contaminant levels compare   Observed concentration vs Ghana
  with safe standards?                Standard

  What is the pH compared with safe   pH range visualization
  drinking water?                     
  -----------------------------------------------------------------------

![Contaminants Breakdown Dashboard](images/contaminants-breakdown.png)

------------------------------------------------------------------------

## 3. Recommendations

The third page translates the analytical findings into potential
response strategies.

Recommendations are organized by:

**Time horizon:** Short-term, Medium-term, Long-term

**Intervention area:**

1.  Water Supply
2.  Public Health
3.  Law Enforcement
4.  Environmental Assessment
5.  Mining Practices & Technology
6.  Monitoring

![Recommendations Dashboard](images/recommendations.png)

------------------------------------------------------------------------

#  Key Findings

### Lead exceeded safety levels in every river sampled

**Lead exceeded the applicable safety level in all 11 rivers sampled.**

### Arsenic contributed the largest share of contamination load

Based on the dashboard's contamination-load calculation:

-   **Arsenic --- 47%**
-   **Chromium --- 38%**
-   **Lead --- 14%**

### Every river exceeded limits for at least two contaminants

All 11 sampled rivers recorded exceedances for **at least two** of the
contaminants assessed.

### River Subri showed the most severe contaminant profile

River Subri recorded:

-   **Chromium: 32.14×** the applicable standard
-   **Cadmium: 4.33×** the applicable standard
-   **Lead: 20.80×** the applicable standard

It was also the **only river** in the dataset with a Cadmium exceedance.

### River Anuru recorded the highest Arsenic exceedance

River Anuru recorded an Arsenic level of **44.4× the national standard**
used in the analysis.

### River Offin showed substantial Chromium and Lead exceedances

-   Chromium: **8.22×**
-   Lead: **14.80×**

### pH levels were below the recommended range

All sampled water samples had pH values below the recommended
**6.5--8.5** range.

The **Galamsey Pit** sample recorded the most extreme acidity, with a pH
of approximately **3.21**.

------------------------------------------------------------------------

#  Exceedance Summary

  Sample           Arsenic   Cadmium   Chromium     Lead
  -------------- --------- --------- ---------- --------
  Ankobra           22.10×        0×      5.86×   11.90×
  Anuru             44.40×        0×      3.00×    6.20×
  Ashrey            36.70×        0×      1.92×    7.90×
  Birim             37.20×        0×      0.74×    6.50×
  Butre             34.10×        0×      2.94×    6.60×
  Galamsey Pit      29.10×        0×      0.42×    5.10×
  Oda               36.40×        0×      2.06×    7.30×
  Offin             21.60×        0×      8.22×   14.80×
  Pra Daboase       28.80×        0×      3.72×    5.70×
  Pra Twifo         30.50×        0×      2.30×   13.30×
  Subri                 0×     4.33×     32.14×   20.80×
  Tano              34.60×        0×      3.74×    8.60×

> **Note:** The Galamsey Pit is included for comparison but is not
> counted as one of the 11 rivers.

------------------------------------------------------------------------

#  Power BI / DAX

The dashboard was developed using Power BI and DAX measures for:

-   Standard-limit lookup
-   Contaminant exceedance
-   Exceedance ratios
-   Exceedance amounts
-   Total Exceedance Index
-   Contaminant-load contribution
-   Rivers with contaminant exceedances
-   Unsafe-river percentage
-   pH exceedance assessment
-   Highest contaminant load

------------------------------------------------------------------------

#  Public Health Relevance

Water contamination can have implications for population health when
contaminated water is used for drinking, food preparation, household
activities, agriculture, or other forms of human exposure.

From a **public health informatics** perspective, this project
demonstrates how environmental health data can be transformed into
information that supports:

-   Identification of potentially affected communities
-   Prioritization of monitoring activities
-   Risk communication
-   Environmental-health surveillance
-   Evidence-informed intervention planning
-   Communication between technical and non-technical stakeholders

The dashboard supports **data-driven situational awareness**. It does
not diagnose individual health conditions or establish causal
relationships between specific river samples and health outcomes.

------------------------------------------------------------------------

#  Why This Project Matters to Public Health Informatics

**Environmental Data + Public Health + Data Analytics + Information
Visualization**

The workflow demonstrates how a public-health data professional can:

1.  Obtain environmental-health data.
2.  Prepare and structure the data.
3.  Apply defined standards.
4.  Quantify deviations from those standards.
5.  Visualize geographic and contaminant patterns.
6.  Communicate findings to decision-makers.
7.  Translate findings into potential response strategies.

------------------------------------------------------------------------

#  Tools & Technologies

-   **Power BI** --- data modeling, DAX calculations and dashboard
    development
-   **Microsoft Excel** --- dataset preparation
-   **DAX** --- analytical measures and exceedance calculations
-   **Data Visualization** --- geographic, comparative and
    indicator-based visualizations


------------------------------------------------------------------------

#  Project Walkthrough

A short walkthrough video demonstrates the dashboard's three pages and
explains the main findings.

**Project walkthrough:**\
[Watch the dashboard walkthrough](https://youtu.be/UVdXCxq_nrg)

------------------------------------------------------------------------

#  Limitations

-   The analysis is based on the available sampled measurements and
    should not automatically be interpreted as representing every river
    or water source in Ghana.
-   The dataset contains sampled locations rather than continuous
    monitoring data.
-   The analysis identifies exceedances against defined standards but
    does not establish causation between mining activity and individual
    health outcomes.
-   The dashboard does not estimate population exposure or disease
    burden.
-   A water-quality exceedance does not by itself establish that a
    specific health outcome will occur in an individual.
-   The Galamsey Pit is a mining-site sample and is analyzed separately
    from the 11 river samples.
-   Findings depend on the standards, measurements, units and sampling
    information available in the source dataset.

------------------------------------------------------------------------

#  Future Improvements

-   Add more sampling locations and sampling periods.
-   Incorporate historical data to identify trends over time.
-   Add population and settlement data to estimate potentially affected
    populations.
-   Integrate rainfall, land-use and mining-location data.
-   Add health-outcome or disease-surveillance data where ethically and
    appropriately available.
-   Develop automated data pipelines for periodic monitoring.
-   Add district/community-level geographic analysis.
-   Incorporate additional environmental parameters and contaminants.
-   Develop an online version of the dashboard.

------------------------------------------------------------------------

#  Key Takeaway

The analysis identifies widespread contaminant and pH exceedances across
the sampled rivers, with particularly notable patterns involving **Lead,
Arsenic and Chromium**, and a pronounced contamination profile in
**River Subri**.

The project demonstrates a complete analytical workflow:

> **Data → Standards → Exceedance Analysis → Visualization → Public
> Health Interpretation → Recommendations**


------------------------------------------------------------------------

## ⭐ Project Status

**Completed --- Power BI Dashboard**

Maintained as part of my data science and public-health informatics
portfolio.

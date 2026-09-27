# Ghana's Rivers in Crisis --- Galamsey Pollution Dashboard

> **Power BI \| Environmental & Public Health Analytics \| Ghana**

An interactive Power BI dashboard examining water-quality contamination
across **11 sampled rivers** alongside a separate **Galamsey Pit** sample, 
and compares contaminant levels against the **Ghana Standard**.

------------------------------------------------------------------------

##  Project Overview

Galamsey and other mining activities can affect water resources through
the introduction of harmful chemicals to the water. This project
analyzes available water-quality measurements to identify where sampled
rivers exceed selected safety limits, determine the severity and
distribution of contaminant exceedances, and translate the findings into
potential response strategies.


- **Purpose:** Explore where sampled water exceeds selected standards,
which contaminants contribute to exceedances, and potential response areas.
- **Data:** Open Data Bank Ghana; 11 river samples plus one mining-site sample.
- **Focus parameters:** Arsenic (As), Cadmium (Cd), Chromium (Cr), Lead (Pb), and pH.
- **Tools:** Power BI, DAX, Microsoft Excel.
- **Dashboard pages:** Rivers Overview · Contaminants Breakdown · Recommendations.

------------------------------------------------------------------------

# Dashboard

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

#  Project Walkthrough

A short walkthrough video demonstrates the dashboard's three pages and
explains the main findings.

**Project walkthrough:**\
[Watch the dashboard walkthrough](https://youtu.be/UVdXCxq_nrg)


------------------------------------------------------------------------

#  Key Findings

- Lead exceeded the analysis benchmark in all 11 sampled rivers.
- Arsenic accounted for 47% of calculated contaminant load, followed by chromium (38%) and lead (14%).
- Every sampled river exceeded limits for at least two assessed contaminants.
- Subri had the highest chromium and lead exceedance ratios and was the only river with a cadmium exceedance.
- All samples had pH below the 6.5–8.5 range; the Galamsey Pit sample had a pH of approximately 3.21.

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


## Important context

These findings describe the available samples and do not establish conditions in every Ghanaian water source, 
prove that mining caused a particular measurement, estimate population exposure, or diagnose health outcomes. 
The Galamsey Pit is a mining-site sample and is not counted among the 11 rivers.


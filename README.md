# Zion-Tech-Hub-Cohort-analysis
Power BI analysis of Zion Tech Hub Cohorts 9 &amp; 10 to identify registration patterns and inform the Cohort 11 paid advertising strategy.
# Zion Tech Hub Cohort 9 & 10 Registration Analysis

## Project Overview

Zion Tech Hub is preparing to launch its first paid advertising campaign to attract registrations for Cohort 11. Since there is no historical paid advertising data, this project analyzes registration data from Cohort 9 and Cohort 10 to identify patterns that can help guide the Cohort 11 campaign strategy.

The analysis focuses on registration volume, acquisition channels, course preferences, geographic distribution, gender, occupation, and registration timing.

The goal is to use historical registration behavior as evidence for deciding where to focus future campaign efforts, while recognizing that registration data alone cannot predict paid advertising performance.

---

## Business Questions

This analysis aims to answer:

1. Where are most registrations coming from?
2. Which acquisition channels generated the most registrations?
3. How did acquisition channels change between Cohort 9 and Cohort 10?
4. Which courses attracted the most registrations?
5. Where are registrants located?
6. What does the gender distribution look like?
7. What occupations are represented among Cohort 10 registrants?
8. Are there noticeable registration patterns over time?
9. What data-backed considerations should Zion Tech Hub use when planning the Cohort 11 campaign?

---

## Dataset

The project uses registration data from:

* Cohort 9
* Cohort 10

The datasets were cleaned separately in Power Query and then appended into one combined dataset.

The final combined dataset contains:

* **1,218 registration records**
* **942 distinct email addresses**

Repeated email addresses were retained because the same email could appear across different registration events with different timestamps, courses, genders, or acquisition sources. Therefore, removing duplicate emails could have removed legitimate registration records.

---

## Data Cleaning and Preparation

The datasets were cleaned and standardized using Power Query in Power BI.

Key cleaning steps included:

* Standardizing column names and data types.
* Cleaning and standardizing email addresses by converting them to lowercase.
* Cleaning the Name field and filling missing Name values using available email information where appropriate.
* Standardizing country values.
* Mapping unclear or inconsistent country entries to **Unclear** rather than making assumptions.
* Standardizing the Program/Course field.
* Cleaning the acquisition source field.
* Standardizing timestamp values by applying the appropriate Nigeria locale.
* Adding a Cohort column to identify Cohort 9 and Cohort 10 after appending the datasets.
* Removing the phone number field because the data was incomplete and not required for the analysis.
* Retaining repeated email addresses because they could represent different registration events.
* Reviewing column quality and ensuring important fields had valid data types.

### Occupation Data

Occupation information was available for Cohort 10 but not Cohort 9.

Because of this, occupation analysis was performed using Cohort 10 data only rather than treating the missing Cohort 9 occupation values as actual missing occupations.

---

## Dashboard

The Power BI dashboard contains several visuals designed to highlight registration patterns across the two cohorts.

### Key Dashboard Visuals

* Total Registrations — Cohort 9 & 10
* Total Registrations by Cohort
* Course Registrations by Cohort
* Country Distribution by Cohort
* Registrations by Acquisition Channel
* Registration by Gender
* Daily Registration Trend
* Cohort 10 Registrations by Occupation

---

## Key Findings

### 1. Registration Volume

The combined dataset contains **1,218 registration records**.

* Cohort 9: **1,047 registrations**
* Cohort 10: **171 registrations**

Cohort 9 therefore has substantially more registration records than Cohort 10.

However, the difference in registration volume should not automatically be interpreted as a decline in interest because the data does not provide enough information to establish why the cohort sizes differ.

---

### 2. Acquisition Channels

The largest recorded acquisition sources were:

* **X (Twitter): 795**
* **WhatsApp: 205**
* **LinkedIn: 167**
* **Referral: 28**
* **Facebook: 14**
* **WhatsApp Community: 5**
* **Instagram: 4**

X (Twitter) was the largest recorded source of registrations in the historical registration data.

However, these figures represent registration sources rather than paid advertising performance. There is no historical data on ad spend, impressions, clicks, cost per click, cost per registration, or paid conversion rates.

---

### 3. Changes in Acquisition Sources

The acquisition mix changed between Cohort 9 and Cohort 10.

X (Twitter) remained an important source across the cohorts, while some other channels changed.

For example:

* WhatsApp and WhatsApp Community appeared in Cohort 9.
* These sources were not recorded in Cohort 10.
* Instagram appeared in Cohort 10.

This suggests that acquisition behavior was not identical across the two cohorts and should be monitored when planning future campaigns.

---

### 4. Geographic Distribution

Nigeria was the largest recorded country source.

There were **718 registration records from Nigeria**:

* Cohort 9: **611**
* Cohort 10: **107**

This indicates that Nigeria represents a major historical registration market within the available data.

However, the country data required cleaning because some entries were inconsistent or unclear. These entries were grouped as **Unclear** instead of being assigned to a country without sufficient evidence.

---

### 5. Course Registrations

Cohort 9 recorded a large number of registrations for **Data Science and AI**, with **465 registration records**.

Cohort 10 included registrations across multiple programs, including:

* Data Science
* Supply Chain Analytics
* AI Automation
* Healthcare Analytics
* Financial Analytics
* Sales & Marketing Analytics

This shows that the course mix expanded in Cohort 10 compared with the available Cohort 9 course data.

---

### 6. Gender Distribution

The registration records were predominantly male:

* Male: **900 (73.89%)**
* Female: **309 (25.37%)**
* Prefer not to say: **9**

This describes the gender distribution within the available registration records. It does not explain why the difference exists or indicate the gender distribution of the wider potential audience.

---

### 7. Occupation

Occupation data was available only for Cohort 10.

Students represented the largest occupation group, followed by groups such as:

* Unemployed
* Data Analyst
* Entrepreneur
* Other/Unspecified occupations

Because Cohort 9 does not contain occupation information, occupation trends cannot reliably be compared between the two cohorts.

---

### 8. Registration Timing

The daily registration trend shows changes in registration volume over time, with noticeable spikes around **January 22–23, 2026**.

These spikes identify periods of higher registration activity, but the available data does not establish what caused those increases.

---

## Business Insights

Based on the registration data, several areas can be considered when planning the Cohort 11 campaign:

### Acquisition

X (Twitter) generated the highest number of historical registrations and should therefore be considered as an important channel to test.

However, the historical data should be treated as a starting point rather than proof that paid advertising on X will produce the best results.

### Geographic Targeting

Nigeria accounted for the largest share of recorded registrations. This provides evidence that Nigeria is an important market within the existing registration base.

### Course Targeting

The data shows demand across several courses, particularly Data Science and AI in Cohort 9, while Cohort 10 showed registrations across a broader range of specialized programs.

Campaign messaging could therefore be adapted to different course interests rather than using one message for every program.

### Audience Expansion

The registration base is predominantly male, while students form a large part of the Cohort 10 occupation data.

This provides an opportunity to examine whether future campaign messaging can reach a broader range of potential participants, including underrepresented groups.

### Timing

The daily registration trend shows periods of increased registration activity. These periods can be monitored when planning future promotional activity, although the current data does not prove that timing caused the spikes.

---

## Data Limitations

Several limitations should be considered when interpreting the analysis:

1. **No historical paid advertising data**
   There is no previous paid campaign data such as ad spend, impressions, clicks, CPC, CPA, or paid conversion rate.

2. **Unequal cohort sizes**
   Cohort 9 contains 1,047 records while Cohort 10 contains 171 records. Raw counts should therefore be interpreted carefully when comparing the cohorts.

3. **Missing occupation data for Cohort 9**
   Occupation analysis is limited to Cohort 10.

4. **Repeated email addresses**
   The dataset contains 1,218 registration records but only 942 distinct email addresses. Repeated emails were retained because they may represent different registration events.

5. **Country inconsistencies**
   Some country entries were unclear or inconsistent and were grouped into an Unclear category rather than being incorrectly classified.

6. **No causal information**
   The dataset shows registration patterns but does not explain why those patterns occurred.

7. **No paid campaign performance data**
   Historical registration sources cannot be directly interpreted as paid advertising performance.

---

## Recommendations for Cohort 11

Based on the available evidence, the Cohort 11 campaign should:

* Use historical acquisition channels as starting points for testing rather than assuming they will produce the same results with paid advertising.
* Consider Nigeria as an important geographic audience based on historical registration records.
* Test different messages for different course interests.
* Monitor acquisition channels separately during the campaign.
* Track impressions, clicks, cost per click, registrations, cost per registration, and conversion rates for every paid channel.
* Compare campaign performance by audience, course, location, and acquisition source.
* Monitor registration activity over time to identify periods of stronger response.
* Collect occupation information consistently across future cohorts.
* Maintain consistent country and acquisition-source categories in future registration forms.
* Use campaign results from Cohort 11 to create a stronger evidence base for future advertising decisions.

---

## Tools Used

* **Microsoft Power BI**
* **Power Query**
* **DAX**
* **Microsoft Excel**

---

## Project Workflow

The project followed these main stages:

1. Collected Cohort 9 and Cohort 10 registration datasets.
2. Cleaned each dataset separately in Power Query.
3. Standardized important fields such as email, country, program, timestamp, and acquisition source.
4. Added cohort labels.
5. Appended the cleaned datasets.
6. Validated the combined dataset.
7. Created Power BI visuals.
8. Analyzed registration patterns.
9. Identified data limitations.
10. Developed evidence-based considerations for the Cohort 11 campaign.

---

## Conclusion

The analysis of Zion Tech Hub Cohort 9 and Cohort 10 registration data provides useful evidence about historical registration patterns.

Nigeria was the largest recorded geographic source, while X (Twitter) was the largest recorded acquisition source. Cohort 9 had substantially more registration records than Cohort 10, while Cohort 10 showed a broader range of course and occupation data.

At the same time, the absence of historical paid advertising data means the existing registration records cannot determine which paid channel will perform best for Cohort 11.

The analysis therefore provides a baseline for campaign testing. By tracking paid campaign performance during Cohort 11, Zion Tech Hub can build a stronger dataset for future advertising decisions.

---

## Author

**Chisom Adiele**

Data Analyst

GitHub: chisomsql

Power BI | Excel | Data Analysis

## Background

The negotiations around the 2017-08-18 contract were quite lengthy.  There were numerous contract revisions leading up to the final version that was signed.  Unfortunately, some good information was accidentally deleted.  This document tries to capture the omitted information around the details of the data delivery contents.  This information was provided to Premier, it just didn't make it into the final version by accident.

## Collaborative Development Disclaimer

*When presenting the base datamart field and table list, the following language was intended to accompany it:*

The following table describes the structure of the basic claims-level DataMart.  This structure will be consistently provided for all clients.  This should be considered a starting point; it is anticipated for the specific structure to be refined through an iterative process to support Premier’s development of any additional reporting or deliverables.

## Extra details around specific data enhancements

*The following descriptions were intended to be included to describe the enhanced data feed options:*

### Milliman CCHGs

Milliman Chronic Conditions Hierarchical Groups (CCHGs) is a unique clinical-care-based identification methodology for patients and chronic conditions designed to more accurately identify cost trend drivers and effectively allocate disease and care management resources. Coupled with traditional actuarial analyses, this highly effective, patient-centric model produces an information-driven management process that results in more effective care and lower administrative costs.

This would be provided as an additional dimension on the members table in the DataMart and a corresponding reference table.  The costs would be waived if the client also purchased ACO Insights – enhanced edition.

### Milliman Waste Calculator

The Milliman Waste Calculator is an analytical tool that provides actionable data to support healthcare quality, efficiency, and effectiveness reporting. The calculator brings together clinical expertise and powerful data analytics—allowing healthcare managers to target and reduce wasteful spending.

This would be provided as an additional dimension on the outclaims table in the DataMart and a corresponding reference table.  The costs would be waived if the client also purchased ACO Insights – enhanced edition.

### Milliman HCG Benchmarks

The Milliman HCG Benchmarks can be used to analyze and benchmark cost and utilization for many different types of population data, such as product lines, lines of business, employer groups, primary care panels, disease populations, incurred service periods, and member state.  For each benchmark, a “Well Managed” and “Loosely Managed” value will be provided.

This would be provided as an additional table with one record per service category and benchmark (e.g. Well Managed Inpatient Surgical Admission).  Each record will contain cost and utilization benchmarks as available.  Additional reference/cross-walk tables will be provided as needed to support summarizing outclaims and outpharmacy to a consistent basis.  The costs would be waived if the client also purchased ACO Insights – enhanced edition.

These benchmarks would be limited to Medicare ACOs at this time.  It would be possible to provide them for other populations under a separate statement of work.

### PRM Opportunity Prospective Scores

The PRM Opportunity Prospective Scores are custom predictive models focused on prioritizing care coordination.  The primary prediction focuses on predicting future Potentially Avoidable Costs.  Additional predictions identify probabilities of inpatient admission or emergency room visits.  The machine learning algorithms underlying these predictions will be re-trained on each data feed, thus adapting to the existing care patterns for each client.

This would be provided as an additional table with one record per member and prediction (e.g. one record for John Doe’s probability of inpatient admission).  Additionally, a table of risk factors for the Potentially Avoidable Cost prediction for each member can be provided.  The costs would be waived if the client also purchased PRM’s Care Coordinator Report.  These scores can only be provided on populations up to 250,000 lives.

### PRM Conditions to Consider

The PRM Conditions to Consider analytics provide insight into the conditions coded on each patient.  Chronic conditions that have not been re-coded during the current performance year are identified and reported.  A unique collaborative filtering algorithm identifies other conditions that have been coded on similar patients.  This collaborative filtering algorithm is re-trained for each client so their own clinical coding patterns are reflected.  Additionally, historical condition information, including likely managing specialists, are also reported.  Conditions are defined using AHRQ’s CCS definitions.

This would be provided as additional tables.  One will be a historic table with one record per member and already coded condition (e.g. one record for John Doe’s Diabetes condition, including the last service date and managing physician).  The other table with be the predictions table with one record per member and condition to consider (e.g. 10 records for John Doe showing the top 10 outputs of the collaborative filtering model for John Doe).  The costs would be waived if the client also purchased PRM’s Care Coordinator Report.

### PRM Medicare ACO Analytics

The PRM Medicare ACO Analytics includes reporting on claims-based quality metrics and MSSP assignment metrics.  For the claims-based quality metrics, patient-level status will be provided, along with a free-text field that provides guidance on the results (e.g. “Last Cholesterol Panel was performed in Dec 2016, which is not in this performance year”).  For the MSSP assignment metrics, information about the relative spend on ACO PCPs vs Non-ACO PCPs will be provided.  This can be used to identify currently assigned patients that are likely to leave the ACO by the end of the performance year, or identify currently un-assigned patients that are likely to join the ACO by the end of the performance year.

The claims-based quality metrics will be provided as an additional table with one record per patient and eligible quality metric (e.g. one record for John Doe’s A1C testing quality metric).  An additional reference table will be provided that gives attributes of each quality metric (e.g. is the metric a binary pass/fail, or an ongoing rate).  The MSSP assignment metrics will be added as dimensions onto the members table.  The costs would be waived if the client also purchased PRM’s Care Coordinator Report.

### Third-Party Claims Episode Grouping

A Third-Party Claims Episode Grouping solution can be included in the DataMart.

This would be provided as an additional dimensions on the outclaims and outpharmacy tables in the DataMart and any corresponding reference tables.

### Industry standard Risk Scores (CMS-HCC or MARA)

*NOTE: The final 2017-08-18 contract did not cover MARA*

Industry standard risk scores can be included in the DataMart.

This would be provided as an additional table with one record per member, score and time period (e.g. John Doe’s CMS-HCC risk score for claims incurred in CY2016 and paid through 1Q2017) in the DataMart and any corresponding reference tables.

### Industry standard Quality Indicators (AHRQ-PQI, AHRQ-PDI, NYU-ED)

*NOTE: This was ultimately referred to as "Key Claims Metrics" in the 2017-08-18 contract.*

This represents the addition of industry standard quality indicators to the claims-level detail in the DataMart.  Algorithms will include: AHRQ-PQI, AHRQ-PDI and NYU-ED).

This would be provided as an additional dimensions on the outclaims table.

### Post-Acute Care and Benchmarks

*NOTE: A description of this data add-on was never drafted/provided.*

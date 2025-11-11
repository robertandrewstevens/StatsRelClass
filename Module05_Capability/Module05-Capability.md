Module 5: Capability
================
Robert A. Stevens
2025-11-10

**Typical Six Sigma Phase:** Measure

**Six Sigma Green Belt Body of Knowledge Subtopic:**

- Process capability studies

- Process performance vs. specification

- Process capability indices

- Process performance indices

- Short-term vs. long-term capability

- Process capability for attributes data

**Six Sigma Green Belt Body of Knowledge Description:**

- Identify, describe, and apply the elements of designing and conducting
  process capability studies, including identifying characteristics,
  identifying specifications and tolerances, developing sampling plans,
  and verifying stability and normality

- Distinguish between natural process limits and specification limits,
  and calculate process performance metrics such as percent defective

- Define, select, and calculate Cp and Cpk, and assess process
  capability

- Define, select, and calculate Pp, Ppk, Cpm, and assess process
  performance

- Describe the assumptions and conventions that are appropriate when
  only short-term data are collected and when only attributes data are
  available

- Describe the changes in relationships that occur when long-term data
  are used, and interpret the relationship between long- and short-term
  capability as it relates to a 1.5 sigma shift

- Compute the sigma level for a process and describe its relationship to
  Ppk

## Homework

Read **Textbook** sections listed below.

Review **Web Links** listed below.

Review **Capability Notes** after the **Exercises** below.

Complete **Exercises** below.

### Textbook:

9 Six Sigma Measurements \[Introduction only\]

9.1 Converting Defect Rates (DPMO or PPM) to Sigma Quality Level Units

9.2 Six Sigma Relationships

9.3 Process Cycle Time

9.4 Yield

9.5 Example 9.1: Yield

9.6 Z Variable Equivalent

9.7 Example 9.2: Z Variable Equivalent

9.18 Six Sigma Assumptions

11 Process Capability and Process Performance Metrics \[Introduction
only\]

11.1 S4/IEE Application Examples: Process Capability/Performance Metrics

11.2 Definitions

11.3 Misunderstandings

11.4 Confusion: Short-term versus Long-term variability

11.5 Calculating Standard Deviation

11.6 Process Capability Indices: Cp and Cpk

11.7 Process Performance Indices: Pp and Ppk

11.8 Process Capability and the Z Distribution

11.10 Cpm Index

11.11 Example 11.1: Process Capability/Performance Indices

11.12 Example 11.2: Process Capability/Performance Indices Study

11.13 Example 11.3: Process Capability/Performance Indices Needs

11.16 Process Capability/Performance for Attribute Data

## Web Links:

Process Analysis: Process (Machine) Capability Analysis

<http://www.statsoft.com/textbook/stathome.html>

NIST/SEMATECH e-Handbook of Statistical Methods Chapter 3: Characterize

<http://www.itl.nist.gov/div898/handbook/>

## Exercises:

A Supplier Quality Engineer was visiting a supplier’s plant that was
having some quality problems and was, as a matter of course, reviewing
each process running in the plant. In one instance control charts were
being maintained for a process making electrical resistors, and the SQE
was given the charts to study. The process had already been deemed to be
showing excellent long-term stability, and the sample measurements were
being routinely collected and charted on the floor. The quality
characteristic being measured is the resistance, the nominal (target)
value being 100 ohms, with a specification of +/- 2 ohms. The data is
provided in “Module04_SPC.xls” tab “Electrical Resistor Data”.

- Estimate the appropriate process capability indices treating the four
  measurements as a rational subgroup (n = 4). Is the process capable?
  Is there any reason to be concerned about this process?

- Now estimate the same process capability indices for each of the four
  “subgroups” individually. Are these processes capable?

- Compare the process capability indices for each “subgroup” of data.
  What do you observe?

## Capability Notes

### Topics

- Introduction

- Definitions

- Process Indices

- Normal Data

- Non-normal Data

- Attribute Data

### Objectives

- Understand
  - “Traditional” process indexes
  - Standard normal transform (Z)
  - Process shifting in estimating capability
  - How to estimate short-term and long-term process capability
- Use and understand Statistica to evaluate process capability data
  - Statistics \> Probability Calculator \> Six Sigma Calculator
  - Statistics \> Industrial Statistics & Six Sigma \> Process Analysis
    \> Process capability analysis & tolerance intervals, raw data
  - Statistics \> Industrial Statistics & Six Sigma \> Quality Control
    Charts \> SixGraph with X-bar & R chart

### References

- Automotive Industry Action Group (AIAG)

  - *Advanced Product Quality Planning (APQP) and Control Plan*
  - *Statistical Process Control (SPC)*
  - *Measurement Systems Analysis (MSA)*
  - *Production Part Approval Process (PPAP)*

- *Understanding Statistical Process Control* by Wheeler and Chambers

- *Advanced Topics in Statistical Process Control* by Wheeler

### Definitions

- Run Chart

- Control Chart

- Rational Subgroup

- Short- and Long-term Variability

- Capability Study

### Run Chart

- What: A visual representation of time series data; a plot of data over
  time

- Why: To monitor a process to see whether or not the long range average
  is changing

- When: Need to determine whether there is a trend over a specified time
  period

- How:

  - Put time metric on the horizontal axis (x-axis)
  - Put measurement being studied on the vertical axis (y-axis)
  - Plot data in order that is was gathered: Time sequence of data
    points is critical
  - Optional: Connect data points for easy identification of sequence
    and interpretation
  - Optional: Draw a straight line across that plot at the average value
    of the measurements

### Control Chart

- What: A run chart with statistically determined Upper Control Limit
  (UCL) and Lower Control Limit (LCL) lines drawn on either side of the
  process average line

- Why: To filter the noise present in a time-series data set in order to
  minimize the following two mistakes:

  - interpreting noise (common cause variation) as if it were a signal,
    i.e. tampering
  - failing to detect a signal (special cause variation) when it is
    present

- When:

  - Determine whether or not a process has been operating in statistical
    control
  - Achieve and maintain statistical control

- How:

  - Construct a run chart for the mean (X) and the range (R) of the data
    in rational subgroups
  - If there are no rational subgroups, use individual values and moving
    range
  - Add process average line and control limits:
    - UCLR = D4\*Mean(R)
    - LCLR = D3\*Mean(R)
    - UCLX = Mean(X) + 3\*Mean(R)/d2
    - LCLX = Mean(X) - 3\*Mean(R)/d2
    - See a statistical process control book for the appropriate values
      of d2, D3 and D4
  - Interpret chart: Process is “out-of-control” if:
    - One or more points fall outside of the control limits on either
      the mean chart or the range chart, or
    - There are non-random patterns of data within the control limits
    - See a statistical process control book for more details

#### Reducing Variation

- Eliminate special-cause variation

- Find cause and prevent recurrence

- Establish statistical control

- Reduce common-cause variation

- Study the system

- Get management involved

- Improve the system

### Rational Subgroup

- A subgroup gathered in such a manner as to give

- Maximum chance for the measurements in each subgroup to be alike

- Maximum chance for the subgroups to differ one from the other

- This subgrouping scheme assumes a desire to determine whether or not a
  process’s variation appears to come from a constant system of chance
  causes

### Goals of Rational Subgrouping

- Want to establish a sampling window small enough to exclude
  systematic, nonrandom influences - special causes

- Want data to exhibit only common cause variation within groups and
  exhibit only special cause variation between groups - if it exists

### Implications of Rational Subgrouping

- If done correctly, averaged standard deviations from the subgroups
  estimate “best case” process capability of the current process

- If there is a significant difference between the averaged standard
  deviations and the total standard deviation, then either the process
  mean and/or variation is changing over time

### Capability Study

- What: Determining if the production process is likely to produce
  product that will meet the customer’s requirements

- Why:

  - Being in-control is not enough; an in-control process can produce
    bad product
  - A capable process produces less bad products than a non-capable
    process with 100% inspection

- When: Need to determine whether a process, given its natural
  variation, is capable of meeting established specifications see APQP &
  PPAP processes

- How:

  - Perform Measurement Systems Analysis
  - Determine whether process is in-control using a control chart
  - If process is in-control, determine whether process is capable
    using:
    - Ppk = min\[(mean - LSL)/3xSigma, (USL - mean)/3xSigma\], Sigma =
      standard deviation of all data (long-term)
    - Cpk = min\[(mean - LSL)/3xSigma, (USL - mean)/3xSigma\], Sigma =
      standard deviation from control chart (short-term)

### Capability Study Steps

1.  Set up the process to your “best guess” best setup and record the
    values of you Key Process Input variables

2.  Identify a reasonable way to create rational subgroups

3.  Run the product over a short period of time to minimize the impact
    of special cause variation as possible - approximately 30 time
    points are the target for data collection

4.  Have your team carefully observe the process and take plenty of
    notes

5.  Measure and record values for the Key Process Output Variable

6.  Run Capability SixGraph and review: Normal Plot, SPC Charts (Check
    for Stability, Accuracy), Histogram

7.  Complete the worksheet

8.  Diagnose for mean shift and variance inflation

9.  Estimate Long-term Capability

10. Develop action plan based on diagnostics

### Questions to Ask About Output Variables

- Is the measurement system adequate?

- For a Key Process Output Variable is: Nominal best, Larger better, or
  Smaller better?

- Is the concern for process centering, process variation, or both?

- What is the baseline for the process variable?

  - Mean
  - Standard Deviation (Sigma)

- Is the Output currently in statistical control?

- Is the Output affected by time?

- Are there multiple Outputs measured?

- What is the priority?

### Process Indices

- Traditional Process Indices

- Capability Ratios

- Cpm

- Z-Transform & PPM

- Impact on Gage R&R

### Traditional Process Indices

- Cp and Pp

- Ratio of the tolerance (the width of the spec limits) to the actual
  spread (the process tolerance)

- Cpk and Ppk

- Ratio of the tolerance (the with of the spec limits) to the actual
  spread, taking into account the process mean relative to the midpoint
  between specifications

- Cp/Cpk differ from Pp/Ppk by the method of estimating Sigma

### Process Variation

- Inherent Process Variation

- Due to common causes only

- Can be estimated from control charts by R-bar/d2, among other things

- Total Process Variation

- Due to both common and special causes

- May be estimated by the sample standard deviation using all of the
  individual readings obtained from either control charts or a process
  study

### Capability vs. Performance

- Process Capability

- The 6\*Sigma range of a process’s inherent variation, for
  statistically stable processes only, where Sigma is usually estimated
  by Rbar/d2

- Use Cp, CPL, CPU or Cpk

- Short-term capability, i.e., “best-case”

- Process Performance

- The 6\*Sigma range of a process’s total variation, where Sigma is
  usually estimated by the sample standard deviation

- Use Pp, PPL, PPU or Ppk

- Long-term performance, i.e., “actual”

### Assumptions

- The data come from a statistically stable process

- The individual measurements come an approximately normal distribution

- The specifications are based on customer requirements

- There exists a willingness to accept the computed index as the “true”
  value

- Ignore sampling variation

- Otherwise use a confidence interval approach

### Capability Ratios

- VOC = Voice-Of-Customer

- VOP = Voice-Of-Process

- Capability Ratio = CR = 1/Cp = Proportion of tolerance (VOC) used by
  short-term process variation (VOP)

- Performance Ratio = PR = 1/Pp = Proportion of tolerance (VOC) used by
  long-term process variation (VOP)

### Cpm

- Based on Taguchi’s Loss Function concept

- More importance is given to target (T)

- Less importance is given to spec limits

- Variation from target is expressed as:

- Process variability (Sigma = standard deviation)

- Process centering (Mean - T)

- Note: Sigma is same as Ppk’s, so Cpm should be called Ppm

### Back to the Process Improvement Plan

- The Process Improvement Plan calls for performing a short-term
  capability study during the Measurement Phase to establish the process
  baseline

- Statistical software process capability tools provide both estimated
  standard deviations to use to calculate Cp, Cpk, Pp, and Ppk

### Short-term Capability Study

- Covers a relatively short period of time (Days, Weeks) consisting of
  30 to 50 data points

### Long-term Capability Study

- Covers a relatively long period of time (Months, Years) consisting of
  100 to 200 or more data points

### Diagnosing Capability Data

- Using Statistica’s Capability SixGraph, we can tell a lot about the
  dynamics of a process

- Can pick up patterns by investigating differences in Cp, Cpk, Pp, and
  Ppk

- We can also see patterns between and within subgroups graphs

### Z-Transform

- General form: Z = (X – Mean)/Sigma

- This transform produces a value from a normal distribution with Mean =
  0 and Sigma = 1

- The value indicates how far the number is from the mean in units of
  standard deviations

- For example, if Z = 2, that would say that the number in question is 2
  standard deviations away from the Mean

- By using this method, we can calculate the proportion of product that
  is out-of-spec based on that product’s output Mean and Sigma

- The task is to determine the area of the normal curve that is outside
  the upper and lower specification limits

- Easily do this by calculating Z-Transform for each spec limit

- Can now calculate the areas below the lower spec and above the upper
  spec using the normal probability function

- Where do we get the probabilities?

- Look at Z-Table or statistical software such as Statistica

  - Statistics \> Probability Calculator \> Distributions \> Z (Normal)

### Relating Z-Transform to Six Sigma

- To achieve Six Sigma, a short-term capability study should show

  - Z(LSL) \< –6
  - Z(USL) \> +6

- This indicates that the mean of the distribution is six standard
  deviations away from the spec limits

- This also implies that Cp & Cpk \> 2.0

### Sigma Level, PPM and Cpk

- PPM = 1,000,000\*\[P(Z \< LSL) + P(Z \> USL)\]

- Add 1.5\*Sigma Shift

### Words of Caution from Donald J. Wheeler & David S. Chambers

- The conversion of capability values into fractions nonconforming is an
  operation that has no contact with reality

- It is nothing more than fantasy, and the results are illusions, if not
  outright delusions

- George Box: All models are wrong, but some are useful

- Cpk, Sigma Level and PPM are based on models of reality, not reality
  itself

- Use to compare processes and show improvement

### Z-Scores and 1.5\*Sigma Shift

- Add the % calculated to be outside the LSL and USL

- Convert the % outside spec to a Z-Score

- Use “Inverse cumulative probability” function

- To estimate long-term capability from short-term capability data,
  subtract 1.5 from the absolute value of the Z-Score

- To estimate short-term capability from long-term data, add 1.5 to the
  absolute value of the Z-Score to determine the Benchmark Sigma

### Normal Data

- Traditional process capability statistics assume the data follow a
  normal distribution

- If using Statistica to analyze the data

  - Statistics \> Industrial Statistics & Six Sigma \> Process Analysis
    \> Process capability analysis & tolerance intervals, raw data
  - Statistics \> Industrial Statistics & Six Sigma \> Quality Control
    Charts \> SixGraph with X-bar & R chart

#### Example

- A camshaft must be 600 +/- 2 mm long to meet engineering
  specifications

- A sample of 100 camshafts was measured for Supplier 1

- 20 subgroups of 5

- See “camshaft.xls” for data

### Non-normal Data

- If the process data does not follow a normal distribution, either
  - Transform to normal and use traditional capability indices
  - Analyze with another distribution and use non-traditional capability
    indices
- If using Statistica to analyze the data
  - Statistics \> Industrial Statistics & Six Sigma \> Process Analysis
    \> Process capability analysis & tolerance intervals, raw data \>
    Distribution tab

### Non-traditional Capability Indices

- For transformed data, use same formulas as normal data
  - Be sure to transform LSL and USL
- Otherwise, calculate % out-of-spec using Cumulative Probability
  Distribution Function, e.g.
  - Weibull: P(X \< x) = 1 - exp\[-(x/a)b\]
  - a = Scale parameter, b = Shape parameter
- Then calculate equivalent Z-Score and Ppk

### Example

- A company that manufactures floor tiles is concerned about warping in
  the tiles

- USL = 8 mm

- To ensure production quality, it measured warping in 10 tiles each day
  for 10 days

- See “tiles.xls” for data

### Attribute Data

- If the data is attribute, then turn into count data and

- Analyze with appropriate control chart

  - Typically “P” or “U” Charts - Covered in Module 7

- Use attribute capability indices

### Attribute Capability Indices

- For P and NP charts, process capability is reflected by the process
  average P-bar

- For C charts, process capability is C-bar, the average number of
  non-conformities in a sample of fixed size n

- For U charts, process capability is U-bar, the average number of
  non-conformities per reporting unit

### Example 1 - Binomial

- Evaluate the responsiveness of a telephone sales department

- How capable it is of answering incoming calls

- The number of calls that were not answered due to sales representative
  unavailability (a defect) were recorded for 20 days

- Also recorded the daily number of incoming calls

- See “Bpcapa.xls” for data

- Defectives = “Unavailable”

- Use sizes in = “Calls”

### Example 2 - Poison

- A wire manufacturer is concerned about the effectiveness of the wire
  insulation process

- Sampled random lengths of electrical wiring and tested them for weak
  spots in their insulation by subjecting them to a test voltage

- Recorded the number of weak spots and the length of each piece of wire

- See “Bpcapa.xls” for data

- Defects = “Weak Spots”

- Use sizes in = “Lengths”

---
layout: post 
title: Data Science
permalink: /ai/datascience
---

Target Audience: _Undergrads / Fresh grads_

There are already a lot of data science articles in the web, but at times you'll realize that they are quite a discordant mix. This list of resources and tips is different as it gives a holistic (both business-centric and technical) view. I guess we can call it full-stack data science ;) 

This page presents an overview of the various aspects of a typical data science project (along with a longer-term view of them). Hidden below is a recommendation of what tools to use.

- [Business Problem and Requirements Analysis](/ai/datascience/problem)
    - Most of the time, it's impossible to get it right. That's why you should always start small and iterate (quickly)
- [Data acquistion](/ai/datascience/dataacqusition)
    - Plan data structures properly, think about what you might possibly need
    - Easier to standardize data than to code for each scenario 
- Visualisation
    - 
- [Modelling](/ai/datascience/modelling)
    - A software engineering approach to data analysis
    * Write to CSV files, save your outputs
    * Write test cases - adopt a test driven approach
    * Watch out for the package version! Need to update from time to time 
- Reporting
    - Make use of preattentive features, story told by viz should be simple and clear 
    - D3.js is interesting but a little too low-level (it's your best bet if you want something highly customizable, if you're just building normal visualisations there will be alternatives like ___)
- Maintaining
    - Building a data pipeline
    - Online learning
    - Failing Loudly: An Empirical Study of Methods for Detecting Dataset Shift
- Career
    - There are too much to learn - adopt a T-shape learning paradigm (know the basics of )
    - Data science is a generic skill - to be useful, **you need to have domain knowledge** 
    - You can get that from internships
    * https://evykassirer.github.io/playing-the-internship-game/
    * https://twitter.com/KateWassum/status/1065404037883846656
- Data-Driven Culture
    - AI Transformation Playbook How to lead your company into the AI era - Landing AI
    - Implementing data-driven change: At the start, we mentioned that insights generated from data have to be actionable. What's even more important is getting the organisation to execute it.
    - However, creating organisational change is not trivial. Incentive -> Monitoring -> Re-inforce 
    - https://www.bain.com/insights/with-advanced-analytics-its-people-not-data-that-stand-in-the-way-of-change
- Limitations and Furture Work
    - Quite often, we do not have big data
    - Thick data
<br><br>

---

<br>
## Tools

There is a huge range of tools / libraries and there isn't really a consensus but the major debate is between Excel, Python and R.

In general, you should pick up the basics for all of them but master either Python or R.
- Master == Proficiency to the extent that you don't need to waste time to google for the basic commands
- Useful Excel formulae / functions: XLOOKUP (to draw information from one sheet to another), Power Pivot, [What-If Analysis tools (Scenario, Goal Seek, Data Table)](https://support.office.com/en-us/article/use-goal-seek-to-find-the-result-you-want-by-adjusting-an-input-value-320cb99e-f4a4-417f-b1c3-4f369d6e66c7?ui=en-US&rs=en-US&ad=US)
- If your data is small enough for Excel, you should use it to do a round of preliminary data exploration before writing any code on Python / R. It's always good to have a glance at the raw data.

#### Excel 
Dataset Size
- Small dataset (Excel can't show more than $2^{20} \approx $ 1 million rows)

Analysis 
- No overly complicated analysis (else it takes eons to open your files)
- Excel sheets are a pain to understand (you need to look at the formulas cell by cell), but **Power Query** gives it a strong 
boost
- Excel has VBA and add-ins like **XLMiner** and **Analysis ToolPak** but Python libraries and R packages are much more user-friendly

Plots
- Plots are easy to generate in Excel, but **Power BI** gives you a much wider range of options

#### Python / R
Dataset Size
- Big dataset (that can't be subdivided, e.g. into days)

Analysis 
- Complicated analysis is always better in code than on Excel - it's easier to read code than formulae
- RStudio feels much more comfortable for data exploration and cleaning than Python (even with Sypder)
- R has a [learning curve](https://www.statmethods.net/about/learningcurve.html) and can be quite a pain at times 
- R's Caret is amazing but other libraries just feel more arcane than Python's libraries
- Python has its own [fair share of quirks](https://github.com/satwikkansal/wtfpython) but still feels cleaner

Plots
- Simple plots are very easy to create (using Matplotlib or Seaborn in Python, ggplot in R)
- Highly customizable but it takes time for both Python and R
- If you get carried away with customising your plots, you'll often hit roadblocks and the documentations aren't always very clear

Last updated: 25 July 2019

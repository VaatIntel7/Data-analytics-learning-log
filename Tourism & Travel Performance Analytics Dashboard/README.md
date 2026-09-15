![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![Data Analytics](https://img.shields.io/badge/Data_Analytics-0047AB?style=for-the-badge)


# Tourism & Travel Performance Analytics Dashboard

A data analysis project exploring **$115M in reported revenue across 46,000 travelers** to understand patterns in travel spending, booking channels, traveler satisfaction, and repeat bookings.

Rather than looking at revenue as a single number, I wanted to explore the questions behind it: **Where is the money coming from? Who is spending it? What appears to influence the travel experience? And what changes when the data is viewed from different angles?**

This project became an exercise in moving from individual metrics toward a more connected understanding of the dataset.

---

## Project Focus

The analysis was organized around three areas:

- **Revenue & booking performance**  
  Exploring destinations, booking channels, trip spending, and seasonal patterns.

- **Traveler experience**  
  Comparing satisfaction across accommodation types, transportation methods, destinations, and travel choices.

- **Traveler behavior**  
  Looking at repeat booking patterns and how they vary across traveler groups.

The goal was not simply to produce charts, but to use the dashboard to ask better questions of the data.

---

## What the Data Revealed

A few patterns stood out during the analysis.

### Accommodation and Satisfaction

Camping and glamping recorded the highest overall satisfaction score at **4.00/5.00**, slightly ahead of traditional 5-star hotel accommodation.

This was one of the more interesting findings because it challenged the assumption that higher accommodation classification necessarily corresponds with higher reported satisfaction.

### Booking Channels

Online Travel Agencies recorded the highest booking volume, with **3,516 bookings**.

However, booking volume alone did not tell the whole story. Direct bookings and travel agents showed stronger revenue performance on a per-customer basis, which made channel comparison more useful than simply ranking channels by bookings.

### Repeat Bookings

Backpackers and group tours had the highest repeat booking rates in the dataset, at **38.7% and 38.6%** respectively.

This raised a further question: are certain traveler types inherently more likely to return, or are there other factors within these groups that could explain the difference?

### Travel Insurance

Insured travelers accounted for approximately **$58.9M in total spend**, compared with **$56.5M** among uninsured travelers.

The difference is interesting, but I treated it as an observation rather than proof that insurance causes higher spending. Other factors could contribute to the relationship.

---

## Dashboard Structure

The dashboard is divided into three perspectives, allowing the same dataset to be viewed from different analytical angles.

### 01. Travel Performance Overview

image

The first view establishes the overall picture:

- **$115M total reported revenue**
- **46,000 travelers**
- Average trip spend
- Monthly revenue patterns
- Top-performing destinations
- Booking channel distribution

Switzerland appeared as the highest-revenue destination, generating approximately **$8M** in the dataset.

### 02. Revenue & Traveler Behaviour

image

The second view moves beyond overall performance to examine relationships between:

- Booking channels and revenue
- Traveler demographics and repeat bookings
- Country-level revenue
- Health and safety perceptions
- Potential differences between traveler groups

This section was particularly useful for seeing how a single KPI can look different once it is segmented.

### 03. Traveler Experience

image

The final view focuses on satisfaction:

- Accommodation type
- Transportation method
- Destination satisfaction
- Eco-friendly choices
- Traveler ratings

Road travel recorded the highest transportation satisfaction score at approximately **3.99/5.00**.

---

## What I Learned Building It

The most valuable part of the project was not any single finding. It was learning how much the presentation and framing of an analysis can change the way the same data is understood.

### From Collecting Metrics to Building a Story

My earlier instinct was to include as many useful metrics as possible.

That approach quickly created visual density without necessarily creating more understanding.

The iteration process pushed me toward a simpler question:

> **What does the viewer actually need to notice first?**

That changed how I approached KPI cards, chart selection, spacing, and the order in which information was presented.

### Choosing the Right Visual

Some visualizations were technically capable of showing the required breakdown but were not necessarily the clearest option.

For example, stacked bar charts provided detailed information about eco-friendly choices, but simpler grouped comparisons made certain differences easier to recognize.

This reinforced an important lesson for me:

**A more detailed chart is not automatically a more informative chart.**

### Working with Crowded Data

Country-level analysis introduced another challenge.

Some geographical groups contained many closely positioned observations, making labels and visual elements difficult to interpret.

Instead of treating the visual as finished simply because all the data was technically present, I had to think about hierarchy, spacing, labeling, and whether the chart was helping or distracting from the question.

### Correlation Is Not Explanation

Several findings in the dataset were interesting enough to suggest possible business questions.

However, an observed relationship is not automatically a causal explanation.

For example, higher spending among insured travelers does not by itself demonstrate that insurance leads travelers to spend more.

Recognizing where the data supports a conclusion, and where it only suggests a question for further investigation, became an important part of the learning process.

---

## Tools & Skills Practiced

### Tools

- Microsoft Excel
- Power BI
- Data visualization
- Data exploration and segmentation

### Analytical Areas Practiced

- KPI development
- Exploratory data analysis
- Revenue analysis
- Customer segmentation
- Comparative analysis
- Trend analysis
- Dashboard layout and visual hierarchy
- Communicating findings through data

---

## Questions I Would Explore Next

The dashboard answers some questions, but it also created new ones.

Some areas I would investigate with additional data include:

- What explains the difference in revenue performance between booking channels?
- Are repeat bookings associated with spending level, destination, accommodation, or traveler demographics?
- Does traveler satisfaction predict repeat booking behavior?
- Why do certain destinations generate significantly more revenue than others?
- How does seasonality differ by destination or traveler segment?
- Is the relationship between insurance and spending still present after controlling for other traveler characteristics?

These would require additional analysis and, in some cases, additional data rather than assumptions from the current dataset.

---

## Project Reflection

This project started as an exercise in building a tourism dashboard and gradually became an exercise in **how to think about data**.

The biggest takeaway was that analysis is not just about finding the largest number, the highest-rated category, or the most attractive chart.

It is about asking what the numbers are actually saying, understanding what they cannot say, and presenting the difference clearly.

That is the part of data analysis I am continuing to develop.

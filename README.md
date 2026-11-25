# 🎓 Udemy Courses Analytics Dashboard


An interactive Power BI dashboard that analyzes Udemy's course catalog — course reach, pricing, engagement, and publishing trends — across 4 connected report pages, styled in Udemy's own purple & black brand and navigable entirely inside the report (no default page tabs needed).

---

## ✨ Features

- 4-page interactive report: Landing Page → Overview → Courses Performance → Publication Analysis
- Custom in-report navigation — action buttons move between pages without using the default Power BI page tabs
- Cross-filtering slicers (Level, Subject) that instantly filter every KPI and chart on the active page
- Dynamic KPI cards for the headline numbers (subscribers, courses, reviews, price, content hours)
- Multiple visual types: scatter chart, donut chart, line chart, clustered bar/column charts, area chart
- Custom brand styling (Udemy purple #A435F0 on black) applied consistently across all pages

## 📊 Pages Breakdown

### 1. Landing Page

![Landing Page](Udemy%20Power%20BI%202%20.png)
Entry point of the report with the Udemy logo and four navigation buttons/cards, each describing and linking to one of the other pages.

### 2. Overview Page

![Overview Page](Udemy%20Power%20BI.png)
High-level snapshot of the whole catalog:
- KPI cards: Total Subscribers, Total Courses, Total Number of Lectures, Total Number of Reviews, AVG Course Price, AVG Course in Hours
- Content Duration vs Subscribers by Payment Type (scatter chart)
- Total Subscribers by is_paid (donut chart)
- Total Subscribers and Total Courses by Year (line/area chart)
- Slicers: Level, Subject

### 3. Courses Performance

![Courses Performance](Udemy%20Power%20BI%203.png)
Deep-dive into how individual courses and categories perform:
- KPI cards: Total Subscribers, Total Number of Lectures, Total Courses, Total Number of Reviews, AVG Course Price, AVG Course in Hours
- Course by Level (column chart)
- Total Lectures by Subject (bar chart)
- Top 10 Content Durations by Subscribers (area/line chart)
- Slicers: Level, Subject

### 4. Publication Analysis

![Publication Analysis](Udemy%20Power%20BI%204.png)
How the catalog has grown over time:
- KPI cards: Total Subscribers, Total Number of Lectures, Total Courses, Total Number of Reviews, Years Range Count
- Courses Published by Year (bar chart)
- Subscribers Growth by Publication Year (column chart)
- Publication Trend Over Years (quarterly area/line chart)
- Slicers: Level, Subject

## 🧮 Key DAX Measures

| Measure | Description |
|---|---|
| Total Courses | Count of courses in the catalog |
| Total Subscribers | Sum of subscribers across courses |
| Total Revenue | Estimated revenue (price × subscribers) |
| AVG Course Price | Average course price |
| AVG Course in Hours | Average content duration |
| Total Number of lectures | Sum of lectures across courses |
| Totla Number of Reviews | Sum of reviews across courses |

## 🧰 Tech Stack

- Power BI Desktop — data modeling, DAX, and report design
- DAX — KPI and aggregation measures
- Power BI native visuals — cards, slicers, scatter/donut/line/bar/column/area charts, action buttons

## 🗂️ Repository Structure

udemy-courses-analytics-dashboard/
├── Udemy.pbix              # Main Power BI report file
├── Udemy Power BI.png      # Overview page screenshot
├── Udemy Power BI 2 .png   # Landing page screenshot
├── Udemy Power BI 3.png    # Courses Performance page screenshot
├── Udemy Power BI 4.png    # Publication Analysis page screenshot
└── README.md                # Project documentation (this file)


## 🚀 Getting Started

1. Install Power BI Desktop (Windows only, free).
2. Download Udemy.pbix from this repository.
3. Open it in Power BI Desktop — the data model and report pages will load automatically.
4. Use the navigation buttons on the Landing Page to explore the other three pages.

## 📈 Data Source

Course-level data on Udemy courses (title, subject, level, price, subscribers, reviews, lectures, content duration, and publish date).

## 🙋 About

Built as a personal Power BI project to practice end-to-end dashboard design: data modeling, DAX measures, custom navigation, and UX/branding inside Power BI.

Feedback and suggestions are welcome — feel free to open an issue or reach out.

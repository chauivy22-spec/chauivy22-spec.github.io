---
permalink: /projects/
title: "Project"
author_profile: true
---
## Project 1: Game Market Pulse — Visualizing Video Game Sales, Genre Trends, and Critical Reception (1980–2024)

**Type:** Course Project / Team Project
**Date:** DASC 5231, Data Visualization
**Team:** Kaviya Appu, Zarina Kalymova, Nawal Kazmi, Ngoc Chau Ngo
**Tools:** Tableau

The video game industry has grown from a small hobby into one of the largest entertainment industries in the world, evolving from arcade machines and physical retail dominance into a market now largely driven by digital downloads and mobile gaming. This project analyzed a dataset of roughly 18,000 video game titles released between 1980 and 2024 to better understand what drives a game's commercial success and how the industry itself has changed over four decades.

Using Tableau, our team built a single interactive dashboard with linked filters for release year and genre, so that a selection made in one view automatically updates every other chart. The dashboard follows a structured narrative: it begins by establishing historical market context, moves into category-level performance across consoles, genres, and publishers, then examines the statistical relationship between critic scores and sales, and finishes with a market efficiency analysis comparing average returns per release across genres and decades.

**Key Insights**
- **A synchronized "Golden Age" (2005–2010):** During the Wii/PS3/Xbox 360 era, game supply and demand rose together, marking the peak of the physical retail market. This tight correlation weakened noticeably after 2010, signaling a structural shift as digital distribution began reshaping the industry.
- **Quality measurably predicts sales:** A linear regression model showed that a 1-point increase in critic score was associated with roughly 340,000 additional units sold (p < 0.0001), with sales accelerating sharply once scores crossed a 7.5-out-of-10 threshold.
- **Market concentration:** A small number of publishers (Activision, EA, Nintendo) and genres (Action, Sports, Shooter) account for a disproportionate share of total sales, while GTA V stands out as a true statistical outlier at 64.29 million units sold — more than double the next closest title.
- **A shift toward "blockbuster" economics:** Average sales per release in genres like Shooters rose in the 2010s even as total release volume fluctuated, suggesting the industry has moved toward fewer, higher-impact releases rather than broad, evenly distributed output.
- **Data limitations shape the story:** Because the dataset primarily captures physical sales, the apparent post-2012 decline likely reflects the shift to digital platforms rather than a genuine contraction of the industry — a reminder that the same numbers can look like decline or transformation depending on what's actually being measured.

**How This Applies in Practice**
This kind of analysis mirrors work done by publishers, platform holders, and investors evaluating where to focus development budgets and marketing spend. The critic-score-to-sales relationship offers a data-backed argument for investing in quality assurance and polish before launch, since even a modest score improvement corresponds to meaningful unit sales gains. The genre and publisher concentration findings are directly useful for market-entry decisions — a smaller studio, for example, could use this kind of dashboard to identify genres with strong historical average sales per release rather than chasing oversaturated blockbuster categories. More broadly, the project illustrates a skill applicable well beyond gaming: building a linked, filterable dashboard that lets a non-technical stakeholder explore a large historical dataset and reach their own conclusions, rather than requiring a data analyst to answer every follow-up question one at a time.



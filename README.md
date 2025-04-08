# marketmindz campaign perfomance

## Project Overview

This documentation outlines the development of a Power BI reporting tool for MarketMindz, a market research firm collaborating with a small retail vendor in the food and beverage sector. The primary goal is to create a Business Intelligence (BI) solution that provides insights into marketing campaign performance, product performance, customer demographics, and the factors influencing campaign success.

## Problem Statement

The client is a small company that is still in the process of understanding its market and evaluating its customer base. They require a BI tool to gain insights from their marketing data, focusing on the following business requirements:

1. How are our six recent marketing campaigns performing?![Market minds campaign perfomance](https://github.com/user-attachments/assets/a150b41c-dd02-4389-b366-7c162a2f8b19)

2. How are our products performing?
3. Who are our customers?![BUYER composition analysis](https://github.com/user-attachments/assets/a08c9aba-6270-40da-ae31-f8c013cff20b)

4. What drives campaign performance and buyer decision-making?![PURCHASE drivers analysis](https://github.com/user-attachments/assets/5712ef07-34b2-45d1-a699-f1b847b1484b)


## Proposed Solution

To address these requirements, we propose developing a Power BI report that connects to a star schema database. This solution will enable the client to visualize and explore their data interactively.

### Key Features

1. **Data Visualizations**: 
   - Utilize a variety of Power BI visualizations such as charts, cards, and key influencers visuals to effectively display data insights.

2. **Interactive Filters**:
   - Implement visual filters including slicers and dropdowns to allow users to explore data by Campaign, Product, and Customer ID.

### Architectural Design - Star Schema![Star Schema](https://github.com/user-attachments/assets/3bf18b42-d65e-459f-850b-16194c30501f)


The star schema design will consist of the following components:

#### Fact Table

- **Fact Table**: This table will capture quantitative data points, including:
  - **Income**: Total revenue generated.
  - **Accepted Campaigns**: Number of campaigns that received positive responses.
  - **Age**: Age metrics of customers or campaign duration.

#### Dimension Tables

1. **Campaign Dimension**:
   - **Accepted_Ind**: Indicator of campaign acceptance.
   - **Campaign**: Name of the marketing campaign.
   - **ID**: Unique identifier for each campaign.

2. **Platform Dimension**:
   - **ID**: Unique identifier for the platform used.
   - **Platform**: Name of the platform (e.g., social media, email).
   - **Quantity**: Number of interactions or engagements per platform.

3. **Products Dimension**:
   - **ID**: Unique identifier for each product.
   - **Product**: Name of the product.
   - **Total Sales**: Total sales figures for each product.

## Business Metrics

To ensure the solution meets stakeholders' expectations, we will focus on the following key business metrics:

- **Campaign ROI**: Return on investment for each marketing campaign, calculated as (Revenue - Cost) / Cost.
- **Customer Acquisition Cost (CAC)**: Total marketing costs divided by the number of new customers acquired.
- **Sales Performance**: Total sales per product, highlighting top-performing items.
- **Customer Segmentation**: Analysis of customer demographics, including age groups, to tailor marketing strategies.

## Tools Used

- **Power BI Desktop**: This tool will be utilized for creating the Power BI report and establishing a connection with the star schema database. It offers robust features for data transformation, visualization, and sharing insights.

## Recommendations

This Power BI storytelling project aims to empower our client with actionable insights derived from their marketing data. By implementing an interactive reporting tool with a clear architectural design, we can help the client better understand their campaigns, products, and customer base, ultimately driving informed decision-making and strategic growth.
By leveraging these insights, MarketMindz can effectively guide their client toward a more data-driven marketing strategy.
